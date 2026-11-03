---
title: is_latest_version method
second_title: GroupDocs.Search for Python via .NET API References
description: "Checks whether the specified directory contains an index of the latest version."
type: docs
url: /python-net/groupdocs.search/indexupdater/is_latest_version/
is_root: false
weight: 1020
---


## is_latest_version {#index_path}

Checks whether the specified directory contains an index of the latest version.

```python
def is_latest_version(self, index_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_path | `str` | The index directory path. |

**Returns:** bool: True if the specified directory contains an index of the latest version; otherwise False.

### Example

```python
from groupdocs.search import IndexUpdater

updater = IndexUpdater()
if updater.is_latest_version("./my_index"):
    print("The index has the current version.")
else:
    print("The index is outdated.")
```

### Aliases

These names call `is_latest_version` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `is_latest_version_file` | `is_latest_version_file(index_path)` |
| `is_latest_version_string` | `is_latest_version_string(index_path)` |

### See Also
* class [`IndexUpdater`](/search/python-net/groupdocs.search/indexupdater/)
