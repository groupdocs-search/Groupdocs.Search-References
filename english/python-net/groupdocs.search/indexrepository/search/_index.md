---
title: search method
second_title: GroupDocs.Search for Python via .NET API References
description: "Searches in all indexes of the repository."
type: docs
url: /python-net/groupdocs.search/indexrepository/search/
is_root: false
weight: 1040
---


## search {#query}

Searches in all indexes of the repository.

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
from groupdocs.search import IndexRepository

# Create a repository and an index
repository = IndexRepository()
index = repository.create("./MyIndex")   # create index in the specified folder
index.add("./documents")               # add documents to the index

# Perform a search across all indexes in the repository
result = repository.search("Einstein")
print(f"Found {len(result)} hits")
```

## search {#query-options}

Searches in all indexes of the repository.

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
from groupdocs.search import IndexRepository
from groupdocs.search.options import SearchOptions

index_folder = "./MyIndex"
documents_folder = "./documents"
query = "Einstein"

repository = IndexRepository()
index = repository.create(index_folder)  # Creating index
index.add(documents_folder)  # Indexing documents

options = SearchOptions()
options.use_case_sensitive_search = True  # Setting flag of case sensitive search

result = repository.search(query, options)  # Searching
```

## search {#query}

Searches in all indexes of the repository.

```python
def search(self, query):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| query | `SearchQuery` | The search query. |

**Returns:** The search result.

### Example

```python
from groupdocs.search import IndexRepository, SearchQuery

repository = IndexRepository()
index = repository.create("./MyIndex")  # Creating index
index.add("./documents")  # Indexing documents

query = SearchQuery.create_word_query("Einstein")
result = repository.search(query)
print(result)
```

## search {#query-options}

Searches in all indexes of the repository.

```python
def search(self, query, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| query | `SearchQuery` | The search query. |
| options | `SearchOptions` | The search options. |

**Returns:** SearchResult: The search result.

### Example

```python
from groupdocs.search import IndexRepository, SearchQuery
from groupdocs.search.options import SearchOptions

index_folder = "./MyIndex"
documents_folder = "./documents"

repository = IndexRepository()
index = repository.create(index_folder)  # Creating index
index.add(documents_folder)  # Indexing documents

options = SearchOptions()
options.use_case_sensitive_search = True  # Enable case‑sensitive search

query = SearchQuery.create_word_query("Einstein")  # Create search query

result = repository.search(query, options)  # Perform search
print(f"Found {len(result)} matches")
```

### Aliases

These names call `search` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `search_file` | `search_file(query, options)`<br>`search_file(query)` |
| `search_string` | `search_string(query, options)`<br>`search_string(query)` |
| `search_search_query` | `search_search_query(query, options)`<br>`search_search_query(query)` |

### See Also
* class [`IndexRepository`](/search/python-net/groupdocs.search/indexrepository/)
