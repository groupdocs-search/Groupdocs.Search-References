---
title: create_lazy method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a lazy-loaded document."
type: docs
url: /python-net/groupdocs.search.common/document/create_lazy/
is_root: false
weight: 1040
---


## create_lazy {#document_source_kind-document_key-document_loader}

Creates a lazy-loaded document.

```python
def create_lazy(cls, document_source_kind, document_key, document_loader):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_source_kind | `DocumentSourceKind` | The document source kind. This value must match the kind of the loaded document. |
| document_key | `str` | The document key. This value must match the key of the loaded document. |
| document_loader | `IDocumentLoader` | The document loader. |

**Returns:** The created document.

### Example

```python
import datetime
import io
import os

from groupdocs.search import Index
from groupdocs.search.common import Document, DocumentSourceKind
from groupdocs.search.options import IndexingOptions


class DocumentLoaderFromFile(object):
    def __init__(self, document_key, path):
        self.document_key = document_key
        self.path = path

    def load_document(self):
        with open(self.path, "rb") as f:
            stream = io.BytesIO(f.read())
        modified = datetime.datetime.fromtimestamp(os.path.getmtime(self.path))
        return Document.create_from_stream(self.document_key, modified, os.path.splitext(self.path)[1], stream)

    def close_document(self):
        pass


document_loader = DocumentLoaderFromFile("lecture", "./documents/lecture.txt")
document = Document.create_lazy(DocumentSourceKind.STREAM, "lecture", document_loader)

index = Index("./index")
index.add([document], IndexingOptions())
```

### See Also
* class [`Document`](/search/python-net/groupdocs.search.common/document/)
