---
title: create_file_extension method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter that skips documents without the specified extensions."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_file_extension/
is_root: false
weight: 1050
---


## create_file_extension {#extensions}

Creates a filter that skips documents without the specified extensions.

```python
def create_file_extension(cls, extensions):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| extensions | `list[str]` | The list of allowable extensions. |

**Returns:** DocumentFilter: A document filter by document extension.

### Example

```python
from groupdocs.search.options import DocumentFilter

# Allow only .htm and .html files
filter = DocumentFilter.create_file_extension(".htm", ".html")
print(filter)
```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
