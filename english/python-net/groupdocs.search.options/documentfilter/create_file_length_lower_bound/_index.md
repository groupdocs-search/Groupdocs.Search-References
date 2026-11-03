---
title: create_file_length_lower_bound method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter that skips documents whose length is less than the specified lower bound."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_file_length_lower_bound/
is_root: false
weight: 1060
---


## create_file_length_lower_bound {#lower_bound}

Creates a filter that skips documents whose length is less than the specified lower bound.

```python
def create_file_length_lower_bound(cls, lower_bound):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| lower_bound | `int` | The lower bound of the document length. |

**Returns:** DocumentFilter: A document filter by document length.

### Example

```python
from groupdocs.search.options import DocumentFilter

filter1 = DocumentFilter.create_file_length_lower_bound(50 * 1024)
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
