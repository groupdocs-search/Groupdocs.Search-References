---
title: add method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds the specified attributes to the specified indexed document."
type: docs
url: /python-net/groupdocs.search.common/attributechangebatch/add/
is_root: false
weight: 1010
---


## add {#path-attributes}

Adds the specified attributes to the specified indexed document.

```python
def add(self, path, attributes):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| path | `str` | The document path. |
| attributes | `list[str]` | The attributes to add. |

### Example

```python
from groupdocs.search.common import AttributeChangeBatch
import os

batch = AttributeChangeBatch()
batch.add(os.path.abspath("./documents/relativity-lecture.pdf"), ["main"])
batch.add(os.path.abspath("./documents/einstein-biography.txt"), ["main", "biography"])
```

## add {#paths-attributes}

Adds the specified attributes to the specified indexed documents.

```python
def add(self, paths, attributes):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| paths | `list[str]` | The documents paths. |
| attributes | `list[str]` | The attributes to add. |

### Example

```python
import os

from groupdocs.search import Index
from groupdocs.search.common import AttributeChangeBatch

index = Index("./index")
index.add("./documents")

batch = AttributeChangeBatch()
batch.add([os.path.abspath("./documents/relativity-lecture.pdf")], ["main"])

# Apply the changes to the index
index.change_attributes(batch)
```

### Aliases

These names call `add` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_file` | `add_file(path, attributes)` |
| `add_string` | `add_string(path, attributes)` |
| `add_files` | `add_files(path, attributes)`<br>`add_files(paths, attributes)` |
| `add_strings` | `add_strings(path, attributes)`<br>`add_strings(paths, attributes)` |

### See Also
* class [`AttributeChangeBatch`](/search/python-net/groupdocs.search.common/attributechangebatch/)
