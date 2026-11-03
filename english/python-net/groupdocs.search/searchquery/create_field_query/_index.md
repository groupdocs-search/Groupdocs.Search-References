---
title: create_field_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds a field to the specified query."
type: docs
url: /python-net/groupdocs.search/searchquery/create_field_query/
is_root: false
weight: 1030
---


## create_field_query {#field_name-query}

Adds a field to the specified query.

```python
def create_field_query(cls, field_name, query):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| field_name | `str` | The field name to search in. |
| query | `SearchQuery` | The query to add the field. |

**Returns:** SearchQuery: A query with the field to search in.

### Example

```python
from groupdocs.search import SearchQuery
from groupdocs.search.options import CommonFieldNames

word_query = SearchQuery.create_word_query("Einstein")
field_query = SearchQuery.create_field_query(CommonFieldNames.CONTENT, word_query)
result = index.search(field_query)
```

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
