---
title: create_modification_time_lower_bound method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter for skipping documents with modification date earlier than the lower bound."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_modification_time_lower_bound/
is_root: false
weight: 1100
---


## create_modification_time_lower_bound {#lower_bound}

Creates a filter for skipping documents with modification date earlier than the lower bound.

```python
def create_modification_time_lower_bound(cls, lower_bound):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| lower_bound | `datetime` | The lower bound of the document modification time. |

**Returns:** A document filter by document modification time.

### Example

```python
import datetime
from groupdocs.search.options import DocumentFilter
filter1 = DocumentFilter.create_modification_time_lower_bound(datetime.datetime(2017, 1, 1))
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
