---
title: create_file_length_upper_bound method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter for skipping documents with the length greater than the upper bound."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_file_length_upper_bound/
is_root: false
weight: 1080
---


## create_file_length_upper_bound {#upper_bound}

Creates a filter for skipping documents with the length greater than the upper bound.

```python
def create_file_length_upper_bound(cls, upper_bound):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| upper_bound | `int` | The upper bound of the document length. |

**Returns:** DocumentFilter: A document filter by document length.

### Example

```python
from groupdocs.search.options import DocumentFilter

# Skip files larger than 8 MB
size_filter = DocumentFilter.create_file_length_upper_bound(8 * 1024 * 1024)
print(size_filter)
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
