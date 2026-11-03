---
title: get_indexed_documents method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets an array of all indexed documents."
type: docs
url: /python-net/groupdocs.search/index/get_indexed_documents/
is_root: false
weight: 1100
---


## get_indexed_documents

Gets an array of all indexed documents.

```python
def get_indexed_documents(self):
    ...
```

**Returns:** list[DocumentInfo]: An array of all indexed documents.

### Example

```python
from groupdocs.search import Index

index = Index("./index")
index.add("./documents")
for doc in index.get_indexed_documents():
    print(doc.file_path)
```

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
