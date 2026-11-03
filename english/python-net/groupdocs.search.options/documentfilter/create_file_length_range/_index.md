---
title: create_file_length_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter for skipping documents out of the specified document length range."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_file_length_range/
is_root: false
weight: 1070
---


## create_file_length_range {#lower_bound-upper_bound}

Creates a filter for skipping documents out of the specified document length range.

```python
def create_file_length_range(cls, lower_bound, upper_bound):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| lower_bound | `int` | The lower bound of the document length. |
| upper_bound | `int` | The upper bound of the document length. |

**Returns:** A document filter by document length.

### Example

```python
from groupdocs.search.options import DocumentFilter

# Skip documents smaller than 100 KB and larger than 5 MB
filter3 = DocumentFilter.create_file_length_range(100 * 1024, 5 * 1024 * 1024)
print(filter3)
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
