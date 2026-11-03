---
title: create_and method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a logical conjunction of the specified filters."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_and/
is_root: false
weight: 1010
---


## create_and {#filters}

Creates a logical conjunction of the specified filters.

```python
def create_and(cls, filters):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| filters | `list[DocumentFilter]` | Iterable of `DocumentFilter` objects to combine. |

**Returns:** A `DocumentFilter` representing the conjunction of the provided filters.

### Example

```python
import datetime
from groupdocs.search import IndexSettings
from groupdocs.search.options import DocumentFilter

settings = IndexSettings()
filter1 = DocumentFilter.create_creation_time_range(
    datetime.datetime(2015, 1, 1), datetime.datetime(2016, 1, 1)
)
filter2 = DocumentFilter.create_file_extension(".txt")
filter3 = DocumentFilter.create_file_length_upper_bound(8 * 1024 * 1024)

final_filter = DocumentFilter.create_and(filter1, filter2, filter3)
settings.document_filter = final_filter

print(settings.document_filter)
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
