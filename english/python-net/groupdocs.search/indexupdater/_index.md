---
title: IndexUpdater class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents an index updater."
type: docs
url: /python-net/groupdocs.search/indexupdater/
is_root: false
weight: 70
---


## IndexUpdater class

Represents an index updater.

- [Update index](https://docs.groupdocs.com/search/python-net/update-index/)

The IndexUpdater type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search/indexupdater/__init__/) | Initializes a new instance of the [`IndexUpdater`](/search/python-net/groupdocs.search/indexupdater/) class. |

### Methods
| Method | Description |
| :- | :- |
| [can_update_version](/search/python-net/groupdocs.search/indexupdater/can_update_version/#index_path) | Checks whether an index in the specified directory can be updated to the latest version. |
| [is_latest_version](/search/python-net/groupdocs.search/indexupdater/is_latest_version/#index_path) | Checks whether the specified directory contains an index of the latest version. |
| [update_version](/search/python-net/groupdocs.search/indexupdater/update_version/#index_path-new_index_path) | Updates an index of an old version to the latest version. |

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

### See Also
* module [`groupdocs.search`](/search/python-net/groupdocs.search/)
