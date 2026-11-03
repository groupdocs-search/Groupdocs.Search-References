---
title: create_numeric_range_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a numeric range query."
type: docs
url: /python-net/groupdocs.search/searchquery/create_numeric_range_query/
is_root: false
weight: 1050
---


## create_numeric_range_query {#start-end}

Creates a numeric range query.

```python
def create_numeric_range_query(cls, start, end):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| start | `int` | The start value of a range. |
| end | `int` | The end value of a range. |

**Returns:** SearchQuery: A numeric range query.

### Example

```python
from groupdocs.search import SearchQuery

# Create a numeric range query for values between 500 and 600
query = SearchQuery.create_numeric_range_query(500, 600)

# Execute the search against an index
results = index.search(query)
```

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
