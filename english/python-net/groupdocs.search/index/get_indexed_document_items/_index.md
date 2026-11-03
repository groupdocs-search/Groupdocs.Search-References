---
title: get_indexed_document_items method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets an array of nested items of the specified document (for container documents such as ZIP, OST, PST)."
type: docs
url: /python-net/groupdocs.search/index/get_indexed_document_items/
is_root: false
weight: 1090
---


## get_indexed_document_items {#document_info}

Gets an array of nested items of the specified document (for container documents such as ZIP, OST, PST).

```python
def get_indexed_document_items(self, document_info):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `DocumentInfo` | The document info. |

**Returns:** list[DocumentInfo]: An array of document items.

### Example

```python
documents = index.get_indexed_documents()
for doc in documents:
    items = index.get_indexed_document_items(doc)  # Getting list of document items
    for item in items:
        print("\t" + item.inner_path)
```

### Aliases

These names call `get_indexed_document_items` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_indexed_document_items_document_info` | `get_indexed_document_items_document_info(document_info)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
