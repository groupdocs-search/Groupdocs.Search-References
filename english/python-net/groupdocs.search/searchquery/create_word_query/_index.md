---
title: create_word_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a simple word query."
type: docs
url: /python-net/groupdocs.search/searchquery/create_word_query/
is_root: false
weight: 1110
---


## create_word_query {#term}

Creates a simple word query.

```python
def create_word_query(cls, term):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| term | `str` | The term to search for. |

**Returns:** SearchQuery: A simple word query.

### Example

```python
from groupdocs.search import SearchQuery

word_query = SearchQuery.create_word_query("theory")
result = index.search(word_query)
```

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
