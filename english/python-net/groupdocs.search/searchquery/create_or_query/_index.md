---
title: create_or_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a combined query that will find all the documents which will be found at least for one of the original queries."
type: docs
url: /python-net/groupdocs.search/searchquery/create_or_query/
is_root: false
weight: 1060
---


## create_or_query {#left_query-right_query}

Creates a combined query that will find all the documents which will be found at least for one of the original queries.

```python
def create_or_query(cls, left_query, right_query):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| left_query | `SearchQuery` | The left child query. |
| right_query | `SearchQuery` | The right child query. |

**Returns:** A combined OR query.

### Example

```python
from groupdocs.search import SearchQuery

word_query1 = SearchQuery.create_word_query("Einstein")
word_query2 = SearchQuery.create_word_query("relativity")
or_query = SearchQuery.create_or_query(word_query1, word_query2)
result2 = index.search(or_query)
```

## create_or_query {#queries}

Creates a combined query that finds documents matching at least one of the original queries.

```python
def create_or_query(cls, queries):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| queries | `list[SearchQuery]` | The child queries. |

**Returns:** A combined OR query.

### Aliases

These names call `create_or_query` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `create_or_query_search_query` | `create_or_query_search_query(left_query, right_query)`<br>`create_or_query_search_query(queries)` |

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
