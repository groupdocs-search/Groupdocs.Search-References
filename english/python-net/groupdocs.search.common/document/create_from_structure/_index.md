---
title: create_from_structure method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a document from a structure that is an array of text fields."
type: docs
url: /python-net/groupdocs.search.common/document/create_from_structure/
is_root: false
weight: 1030
---


## create_from_structure {#document_key-modification_date-fields}

Creates a document from a structure that is an array of text fields.

```python
def create_from_structure(cls, document_key, modification_date, fields):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_key | `str` | The document key. |
| modification_date | `datetime` | The document modification date. |
| fields | `list[DocumentField]` | The document fields. |

**Returns:** Document: The created document.

### Example

```python
import datetime
from groupdocs.search.common import Document, DocumentField
from groupdocs.search.options import CommonFieldNames

with open(document_file_path, encoding="utf-8") as f:
    text = f.read()

fields = [DocumentField(CommonFieldNames.CONTENT, text)]
document = Document.create_from_structure(
    "ExampleDocument",
    datetime.datetime.now(),
    fields,
)
```

### See Also
* class [`Document`](/search/python-net/groupdocs.search.common/document/)
