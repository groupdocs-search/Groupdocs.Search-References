---
title: get_indexed_documents method
second_title: GroupDocs.Search for Python via .NET API References
description: "Returns an array of all indexed documents."
type: docs
url: /python-net/groupdocs.search.scaling/searcher/get_indexed_documents/
is_root: false
weight: 1030
---


## get_indexed_documents {#shard_index}

Returns an array of all indexed documents.

```python
def get_indexed_documents(self, shard_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| shard_index | `int` | The shard index. |

**Returns:** list[GroupDocs.Search.Scaling.IndexedDocumentInfo]: An array of all indexed documents.

### Example

```python
from groupdocs.search.scaling import Searcher

# Assuming a Searcher instance is already configured for the desired network
documents = searcher.get_indexed_documents(shardIndex=0)
print(f"Indexed documents: {len(documents)}")
```

### Aliases

These names call `get_indexed_documents` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_indexed_documents_int32` | `get_indexed_documents_int32(shard_index)` |

### See Also
* class [`Searcher`](/search/python-net/groupdocs.search.scaling/searcher/)
