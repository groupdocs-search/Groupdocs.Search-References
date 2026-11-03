---
title: create_creation_time_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter that skips documents whose creation date is outside the specified range."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_creation_time_range/
is_root: false
weight: 1030
---


## create_creation_time_range {#lower_bound-upper_bound}

Creates a filter that skips documents whose creation date is outside the specified range.

```python
def create_creation_time_range(cls, lower_bound, upper_bound):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| lower_bound | `datetime` | The lower bound of the document creation time (`datetime.datetime`). |
| upper_bound | `datetime` | The upper bound of the document creation time (`datetime.datetime`). |

**Returns:** A document filter that filters by document creation time.

### Example

```python
import datetime
from groupdocs.search.options import DocumentFilter

# Include only documents created between Jan 1, 2020 and Dec 31, 2020
filter = DocumentFilter.create_creation_time_range(
    datetime.datetime(2020, 1, 1),
    datetime.datetime(2020, 12, 31)
)

print(filter)
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
