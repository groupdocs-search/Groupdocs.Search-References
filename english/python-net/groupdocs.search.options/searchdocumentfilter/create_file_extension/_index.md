---
title: create_file_extension method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter for skipping documents that are not in the specified list of possible extensions."
type: docs
url: /python-net/groupdocs.search.options/searchdocumentfilter/create_file_extension/
is_root: false
weight: 1030
---


## create_file_extension {#extensions}

Creates a filter for skipping documents that are not in the specified list of possible extensions.

```python
def create_file_extension(cls, extensions):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| extensions | `list[str]` | The list of possible extensions. |

**Returns:** A search document filter by document extension.

### Example

```python
from groupdocs.search.options import SearchDocumentFilter

# Include only FB2 and EPUB documents in the search results
document_filter = SearchDocumentFilter.create_file_extension(".fb2", ".epub")
```

### See Also
* class [`SearchDocumentFilter`](/search/python-net/groupdocs.search.options/searchdocumentfilter/)
