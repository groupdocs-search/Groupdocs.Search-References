---
title: create_and_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a combined query that will find only documents which will be found for each original query."
type: docs
url: /python-net/groupdocs.search/searchquery/create_and_query/
is_root: false
weight: 1010
---


## create_and_query {#left_query-right_query}

Creates a combined query that will find only documents which will be found for each original query.

```python
def create_and_query(cls, left_query, right_query):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| left_query | `SearchQuery` | The left child query. |
| right_query | `SearchQuery` | The right child query. |

**Returns:** A combined AND query.

### Example

```python
from groupdocs.search import SearchQuery

# Build individual word queries
word_query1 = SearchQuery.create_word_query("theory")
word_query2 = SearchQuery.create_word_query("relativity")

# Combine them with AND
and_query = SearchQuery.create_and_query(word_query1, word_query2)

# Execute the search
result = index.search(and_query)
```

## create_and_query {#queries}

Creates a combined query that will find only documents which will be found for each original query.

```python
def create_and_query(cls, queries):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| queries | `list[SearchQuery]` | The child queries. |

**Returns:** A combined AND query.

### Aliases

These names call `create_and_query` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `create_and_query_search_query` | `create_and_query_search_query(left_query, right_query)`<br>`create_and_query_search_query(queries)` |

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
