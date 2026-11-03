---
title: check_segments method
second_title: GroupDocs.Search for Python via .NET API References
description: "Checks the index for damaged segment files on the disk and optionally fixes index functionality if fix_index_functionality is True."
type: docs
url: /python-net/groupdocs.search/index/check_segments/
is_root: false
weight: 1030
---


## check_segments {#fix_index_functionality}

Checks the index for damaged segment files on the disk and optionally fixes index functionality if `fix_index_functionality` is True.

```python
def check_segments(self, fix_index_functionality):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| fix_index_functionality | `bool` | The index functionality fix flag. |

### Example

```python
from groupdocs.search import Index

index = Index("path/to/index")

# Check for damaged segments without fixing functionality
index.check_segments(fix_index_functionality=False)

# Check and attempt to fix functionality
index.check_segments(fix_index_functionality=True)
```

### Aliases

These names call `check_segments` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `check_segments_boolean` | `check_segments_boolean(fix_index_functionality)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
