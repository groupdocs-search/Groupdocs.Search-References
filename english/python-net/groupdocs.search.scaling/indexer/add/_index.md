---
title: add method
second_title: GroupDocs.Search for Python via .NET API References
description: "Indexes documents from streams or structures."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/add/
is_root: false
weight: 1010
---


## add {#documents-passwords-options}

Indexes documents from streams or structures.

```python
def add(self, documents, passwords, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| documents | `List[Document]` | The documents from stream or structure. |
| passwords | `List[str]` | The document passwords. |
| options | `IndexingOptions` | The add options. |

### Example

```python
import datetime
import os

from groupdocs.search.common import Document
from groupdocs.search.options import IndexingOptions

# `node` is the master node of a configured and started search network
indexer = node.indexer

file_path = "./documents/document.pdf"
with open(file_path, "rb") as stream:
    document = Document.create_from_stream(
        os.path.basename(file_path),
        datetime.datetime.fromtimestamp(os.path.getmtime(file_path)),
        ".pdf",
        stream)
    # One password per document; None for a document without one
    indexer.add([document], [None], IndexingOptions())
```

## add {#data-options}

Performs an indexing operation and adds the extracted data to the search network.

```python
def add(self, data, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| data | `List[ExtractedData]` | The extracted data. |
| options | `IndexingOptions` | The indexing options. |

### Aliases

These names call `add` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_ilist` | `add_ilist(documents, passwords, options)`<br>`add_ilist(data, options)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
