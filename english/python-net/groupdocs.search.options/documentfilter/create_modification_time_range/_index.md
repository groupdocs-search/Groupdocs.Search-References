---
title: create_modification_time_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter for skipping documents with modification date out of the specified range."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_modification_time_range/
is_root: false
weight: 1110
---


## create_modification_time_range {#lower_bound-upper_bound}

Creates a filter for skipping documents with modification date out of the specified range.

```python
def create_modification_time_range(cls, lower_bound, upper_bound):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| lower_bound | `datetime` | The lower bound of the document modification time. |
| upper_bound | `datetime` | The upper bound of the document modification time. |

**Returns:** DocumentFilter: A document filter by document modification time.

### Example

```python
import datetime
from groupdocs.search.options import DocumentFilter

filter = DocumentFilter.create_modification_time_range(
    datetime.datetime(2017, 1, 1),
    datetime.datetime(2018, 6, 15)
)
print(filter)
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
