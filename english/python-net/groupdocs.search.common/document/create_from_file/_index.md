---
title: create_from_file method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a document from a file."
type: docs
url: /python-net/groupdocs.search.common/document/create_from_file/
is_root: false
weight: 1010
---


## create_from_file {#file_path}

Creates a document from a file.

```python
def create_from_file(cls, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The document file path. |

**Returns:** Document: The created document.

### Example

```python
from groupdocs.search.common import Document

document = Document.create_from_file(document_file_path)
```

### See Also
* class [`Document`](/search/python-net/groupdocs.search.common/document/)
