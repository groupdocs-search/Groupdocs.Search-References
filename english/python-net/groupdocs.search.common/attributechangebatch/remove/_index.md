---
title: remove method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes the specified attributes from the specified indexed document."
type: docs
url: /python-net/groupdocs.search.common/attributechangebatch/remove/
is_root: false
weight: 1040
---


## remove {#path-attributes}

Removes the specified attributes from the specified indexed document.

```python
def remove(self, path, attributes):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| path | `str` | The document path. |
| attributes | `list[str]` | The attributes to remove. |

### Example

```python
import os

from groupdocs.search import Index
from groupdocs.search.common import AttributeChangeBatch

index = Index("./index")
index.add("./documents")

batch = AttributeChangeBatch()
batch.remove(os.path.abspath("./documents/relativity-lecture.pdf"), ["main"])
index.change_attributes(batch)
```

## remove {#paths-attributes}

Removes the specified attributes from the specified indexed documents.

```python
def remove(self, paths, attributes):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| paths | `list[str]` | The documents paths. |
| attributes | `list[str]` | The attributes to remove. |

### Aliases

These names call `remove` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `remove_file` | `remove_file(path, attributes)` |
| `remove_string` | `remove_string(path, attributes)` |
| `remove_files` | `remove_files(path, attributes)`<br>`remove_files(paths, attributes)` |
| `remove_strings` | `remove_strings(path, attributes)`<br>`remove_strings(paths, attributes)` |

### See Also
* class [`AttributeChangeBatch`](/search/python-net/groupdocs.search.common/attributechangebatch/)
