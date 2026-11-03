---
title: update_version method
second_title: GroupDocs.Search for Python via .NET API References
description: "Updates an index of an old version to the latest version."
type: docs
url: /python-net/groupdocs.search/indexupdater/update_version/
is_root: false
weight: 1030
---


## update_version {#index_path-new_index_path}

Updates an index of an old version to the latest version.

Depending on the old version, the index data are converted or its documents are re‑indexed; in the latter case the source documents must be available at their original paths. The updated index is written to `new_index_path`, while the original index at `index_path` remains unchanged.

```python
def update_version(self, index_path, new_index_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_path | `str` | The index directory path. |
| new_index_path | `str` | The directory for the updated index. If the index can be updated, the directory is created if it does not exist; otherwise its content is deleted before the updated index is written. When the update fails, the content may already be deleted. |

**Returns:** VersionUpdateResult: The result of the index version update operation.

| Raises | Description |
| :- | :- |
| `ValueError` | If `new_index_path` is empty, or it is the same as `index_path`, a parent directory of it, or a directory that contains part of the index data. |
| `IOError` | If a file or directory of the index or `new_index_path` cannot be accessed, or if the index in `index_path` is damaged and cannot be converted. |
| `PermissionError` | If access to a file or directory of the index or `new_index_path` is denied. |

### Example

```python
from groupdocs.search import Index, IndexUpdater
from groupdocs.search.common import VersionUpdateResult

source = "./old_index"
target = "./new_index"

updater = IndexUpdater()
if updater.can_update_version(source):
    result = updater.update_version(source, target)
    if result == VersionUpdateResult.UPDATED:
        index = Index(target)
        print(f"Updated index contains {len(index.get_indexed_documents())} documents")
```

### Aliases

These names call `update_version` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `update_version_file` | `update_version_file(index_path, new_index_path)` |
| `update_version_string` | `update_version_string(index_path, new_index_path)` |

### See Also
* class [`IndexUpdater`](/search/python-net/groupdocs.search/indexupdater/)
