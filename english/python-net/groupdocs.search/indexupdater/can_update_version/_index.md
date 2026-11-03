---
title: can_update_version method
second_title: GroupDocs.Search for Python via .NET API References
description: "Checks whether an index in the specified directory can be updated to the latest version."
type: docs
url: /python-net/groupdocs.search/indexupdater/can_update_version/
is_root: false
weight: 1010
---


## can_update_version {#index_path}

Checks whether an index in the specified directory can be updated to the latest version.

```python
def can_update_version(self, index_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_path | `str` | The index directory path. |

**Returns:** bool: True if an index in the specified directory can be updated to the latest version; otherwise False.

### Example

```python
from groupdocs.search import IndexUpdater

updater = IndexUpdater()
if updater.can_update_version("./old_index"):
    print("The index can be updated.")
else:
    print("The index is already up to date or cannot be updated.")
```

### Aliases

These names call `can_update_version` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `can_update_version_file` | `can_update_version_file(index_path)` |
| `can_update_version_string` | `can_update_version_string(index_path)` |

### See Also
* class [`IndexUpdater`](/search/python-net/groupdocs.search/indexupdater/)
