---
title: get_indexed_document method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets an indexed document by document key."
type: docs
url: /python-net/groupdocs.search/index/get_indexed_document/
is_root: false
weight: 1080
---


## get_indexed_document {#document_key}

Gets an indexed document by document key.

The method accepts the file path of a document indexed from a file (as returned by [`DocumentInfo.file_path`](/search/python-net/groupdocs.search.results/documentinfo/file_path/), which is a full path) or the key of a document indexed from a stream or a structure, and returns `None` if there is no such document in the index.

```python
def get_indexed_document(self, document_key):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_key | `str` | The document key. |

**Returns:** The indexed document.

### Example

```python
from groupdocs.search import Index

index = Index("./index")
doc = index.get_indexed_document("example.docx")
if doc is not None:
    print(doc.file_path)
```

### Aliases

These names call `get_indexed_document` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_indexed_document_file` | `get_indexed_document_file(document_key)` |
| `get_indexed_document_string` | `get_indexed_document_string(document_key)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
