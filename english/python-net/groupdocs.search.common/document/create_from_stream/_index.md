---
title: create_from_stream method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a document from a stream."
type: docs
url: /python-net/groupdocs.search.common/document/create_from_stream/
is_root: false
weight: 1020
---


## create_from_stream {#document_key-modification_date-extension-stream}

Creates a document from a stream.

```python
def create_from_stream(cls, document_key, modification_date, extension, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_key | `str` | The document key. |
| modification_date | `datetime` | The document modification date. |
| extension | `str` | The document extension. The extension must start with the period character '.'. |
| stream | `io.RawIOBase` | The document stream. |

**Returns:** Document: The created document.

### Example

```python
import datetime
from groupdocs.search.common import Document

document_path = "path/to/file.pdf"
with open(document_path, "rb") as stream:
    doc = Document.create_from_stream(
        document_key=document_path,
        modification_date=datetime.datetime.now(),
        extension=".pdf",
        stream=stream,
    )
```

### See Also
* class [`Document`](/search/python-net/groupdocs.search.common/document/)
