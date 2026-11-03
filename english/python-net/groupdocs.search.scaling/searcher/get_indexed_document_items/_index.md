---
title: get_indexed_document_items method
second_title: GroupDocs.Search for Python via .NET API References
description: "Retrieves an array of nested items for the specified document (e.g., container documents such as ZIP, OST, PST)."
type: docs
url: /python-net/groupdocs.search.scaling/searcher/get_indexed_document_items/
is_root: false
weight: 1020
---


## get_indexed_document_items {#document_info}

Retrieves an array of nested items for the specified document (e.g., container documents such as ZIP, OST, PST).

```python
def get_indexed_document_items(self, document_info):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `NetworkDocumentInfo` | The document info. |

**Returns:** list[GroupDocs.Search.Results.DocumentItem]: An array of document items.

### Example

```python
import os
from groupdocs.search import Index

index = Index("path/to/index")
for doc in index.get_indexed_documents():
    print(os.path.basename(doc.file_path))
    items = index.get_indexed_document_items(doc)
    for item in items:
        print("\t" + item.inner_path)
```

### Aliases

These names call `get_indexed_document_items` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_indexed_document_items_network_document_info` | `get_indexed_document_items_network_document_info(document_info)` |

### See Also
* class [`Searcher`](/search/python-net/groupdocs.search.scaling/searcher/)
