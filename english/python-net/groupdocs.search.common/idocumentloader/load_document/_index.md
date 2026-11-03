---
title: load_document method
second_title: GroupDocs.Search for Python via .NET API References
description: "Loads a document."
type: docs
url: /python-net/groupdocs.search.common/idocumentloader/load_document/
is_root: false
weight: 1020
---


## load_document

Loads a document.

```python
def load_document(self):
    ...
```

**Returns:** The loaded document.

### Example

```python
import io
import os
from groupdocs.search.common import IDocumentLoader

class MyDocumentLoader(IDocumentLoader):
    def __init__(self, file_path):
        self.file_path = file_path
        self.document_key = os.path.basename(file_path)

    def close_document(self):
        pass

    def load_document(self):
        extension = os.path.splitext(self.file_path)[1]
        with open(self.file_path, "rb") as f:
            buffer = f.read()
        return io.BytesIO(buffer)
```

### See Also
* class [`IDocumentLoader`](/search/python-net/groupdocs.search.common/idocumentloader/)
