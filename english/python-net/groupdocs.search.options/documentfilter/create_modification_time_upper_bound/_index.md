---
title: create_modification_time_upper_bound method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter for skipping documents with modification dates later than the upper bound."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_modification_time_upper_bound/
is_root: false
weight: 1120
---


## create_modification_time_upper_bound {#upper_bound}

Creates a filter for skipping documents with modification dates later than the upper bound.

```python
def create_modification_time_upper_bound(cls, upper_bound):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| upper_bound | `datetime` | The upper bound of the document modification time. |

**Returns:** A document filter by document modification time.

### Example

```python
import datetime
from groupdocs.search.options import DocumentFilter

# Skip documents modified after June 15, 2018
filter2 = DocumentFilter.create_modification_time_upper_bound(
    datetime.datetime(2018, 6, 15)
)
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
