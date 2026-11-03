---
title: create_date_range_query method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a date range query."
type: docs
url: /python-net/groupdocs.search/searchquery/create_date_range_query/
is_root: false
weight: 1020
---


## create_date_range_query {#start-end}

Creates a date range query.

```python
def create_date_range_query(cls, start, end):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| start | `datetime` | The start value of a range. |
| end | `datetime` | The end value of a range. |

**Returns:** SearchQuery: A date range query.

### Example

```python
import datetime
from groupdocs.search import SearchQuery

query = SearchQuery.create_date_range_query(
    datetime.datetime(2017, 1, 1),
    datetime.datetime(2019, 12, 31)
)
result = index.search(query)
```

### See Also
* class [`SearchQuery`](/search/python-net/groupdocs.search/searchquery/)
