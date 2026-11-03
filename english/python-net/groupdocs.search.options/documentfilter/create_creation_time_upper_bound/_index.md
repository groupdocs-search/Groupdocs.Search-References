---
title: create_creation_time_upper_bound method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter for skipping documents with a creation date later than the upper bound."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_creation_time_upper_bound/
is_root: false
weight: 1040
---


## create_creation_time_upper_bound {#upper_bound}

Creates a filter for skipping documents with a creation date later than the upper bound.

```python
def create_creation_time_upper_bound(cls, upper_bound):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| upper_bound | `datetime` | The upper bound of the document creation time. |

**Returns:** A document filter by document creation time.

### Example

```python
import datetime
from groupdocs.search.options import DocumentFilter
filter2 = DocumentFilter.create_creation_time_upper_bound(datetime.datetime(2018, 6, 15))
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
