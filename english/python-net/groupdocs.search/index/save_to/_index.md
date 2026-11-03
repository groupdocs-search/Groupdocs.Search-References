---
title: save_to method
second_title: GroupDocs.Search for Python via .NET API References
description: "Saves the in‑memory or regular index to a specified folder on disk without changing its settings."
type: docs
url: /python-net/groupdocs.search/index/save_to/
is_root: false
weight: 1190
---


## save_to {#index_folder}

Saves the in‑memory or regular index to a specified folder on disk without changing its settings.

An index of the current version that the folder contains is replaced by the saved index.

```python
def save_to(self, index_folder):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The path to the index folder to save. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The folder is the folder of this index, or it contains an index that is not replaced: an index of another version or a damaged index. |

### Example

```python
from groupdocs.search import Index

# Create an in‑memory index
index = Index()

# ... perform indexing operations ...

# Save the index to a folder on disk
index.save_to("./indexes/my_index")
```

### Aliases

These names call `save_to` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `save_to_file` | `save_to_file(index_folder)` |
| `save_to_string` | `save_to_string(index_folder)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
