---
title: delete method
second_title: GroupDocs.Search for Python via .NET API References
description: "Deletes indexed documents."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/delete/
is_root: false
weight: 1030
---


## delete {#document_keys-options}

Deletes indexed documents.

```python
def delete(self, document_keys, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_keys | `list[str]` | The keys of documents added from streams or structures. |
| options | `DeleteOptions` | The delete options. |

### Example

```python
from groupdocs.search.options import DeleteOptions

# `node` is the master node of a configured and started search network
indexer = node.indexer

# Keys of the documents to remove
document_keys = ["doc1", "doc2"]

# Delete the specified documents from the search network
indexer.delete(document_keys, DeleteOptions())
```

### Aliases

These names call `delete` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `delete_files` | `delete_files(document_keys, options)` |
| `delete_strings` | `delete_strings(document_keys, options)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
