---
title: search method
second_title: GroupDocs.Search for Python via .NET API References
description: "Searches in index."
type: docs
url: /python-net/groupdocs.search/index/search/
is_root: false
weight: 1200
---


## search {#query}

Searches in index.

```python
def search(self, query):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| query | `str` | The search query. |

**Returns:** SearchResult: The search result.

### Example

```python
from groupdocs.search import Index

# Create an index and add documents
index = Index("./index")
index.add("./documents")

# Simple text search
result = index.search("Einstein")
print("Documents found:", result.document_count)

# Regular expression search (a query that starts with ^)
regex_result = index.search("^[0-9]{3,}")
print("Documents found:", regex_result.document_count)

# Faceted search (a field name followed by a colon)
faceted_result = index.search("content:Newton")
print("Documents found:", faceted_result.document_count)
```

## search {#query-options}

Searches in the index.

```python
def search(self, query, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| query | `str` | The search query. |
| options | `SearchOptions` | The search options. |

**Returns:** SearchResult: The search result.

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import SearchOptions
from groupdocs.search.options import TableDiscreteFunction

# Create or open an index
index = Index("./index")
# Index documents from a folder
index.add("./documents")

# --- Fuzzy search example ---
fuzzy_options = SearchOptions()
fuzzy_options.fuzzy_search.enabled = True
fuzzy_options.fuzzy_search.fuzzy_algorithm = TableDiscreteFunction(1)

fuzzy_query = '"The Pursuit of Happiness"'
fuzzy_result = index.search(fuzzy_query, fuzzy_options)

# --- Synonym search example ---
synonym_options = SearchOptions()
synonym_options.use_synonym_search = True

synonym_query = "cry"
synonym_result = index.search(synonym_query, synonym_options)
```

## search {#query}

Searches in index.

```python
def search(self, query):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| query | `SearchQuery` | The search query. |

**Returns:** SearchResult: The search result.

### Example

```python
    from groupdocs.search import Index, SearchQuery
    from groupdocs.search.options import SearchOptions
    from groupdocs.search.options import TableDiscreteFunction

    index = Index("./index")
    index.add("./documents")

    # Subquery 1: word query with fuzzy search enabled
    subquery1 = SearchQuery.create_word_query("accommodation")
    subquery1.search_options = SearchOptions()
    subquery1.search_options.fuzzy_search.enabled = True
    subquery1.search_options.fuzzy_search.fuzzy_algorithm = TableDiscreteFunction(3)

    # Subquery 2: numeric range query
    subquery2 = SearchQuery.create_numeric_range_query(1, 1_000_000)

    # Subquery 3: regex query
    subquery3 = SearchQuery.create_regex_query(r"(.)\1")

    # Combine subqueries into a phrase query
    query = SearchQuery.create_phrase_search_query(subquery1, subquery2, subquery3)

    result = index.search(query)
    ```

## search {#query-options}

Searches in index.

```python
def search(self, query, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| query | `SearchQuery` | The search query. |
| options | `SearchOptions` | The search options. |

**Returns:** SearchResult: The search result.

## search {#image-options}

Performs a reverse image search in the index.

```python
def search(self, image, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| image | `SearchImage` | The image to search. |
| options | `ImageSearchOptions` | The image search options. |

**Returns:** The result of a reverse image search.

### Aliases

These names call `search` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `search_file` | `search_file(query, options)`<br>`search_file(query)` |
| `search_string` | `search_string(query, options)`<br>`search_string(query)` |
| `search_search_query` | `search_search_query(query, options)`<br>`search_search_query(query)` |
| `search_search_image` | `search_search_image(image, options)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
