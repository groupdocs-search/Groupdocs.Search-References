---
title: change_attributes method
second_title: GroupDocs.Search for Python via .NET API References
description: "Applies the specified batch of attribute changes to indexed documents without reindexing during the update operation."
type: docs
url: /python-net/groupdocs.search/index/change_attributes/
is_root: false
weight: 1020
---


## change_attributes {#batch}

Applies the specified batch of attribute changes to indexed documents without reindexing during the update operation.

```python
def change_attributes(self, batch):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| batch | `AttributeChangeBatch` | The attribute change batch. |

### Example

```python
import os

from groupdocs.search import Index
from groupdocs.search.common import AttributeChangeBatch

with Index("./index") as index:
    index.add("./documents")

    batch = AttributeChangeBatch()
    batch.add([os.path.abspath("./documents/lecture.txt")], ["main"])
    index.change_attributes(batch)
```

### Aliases

These names call `change_attributes` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `change_attributes_attribute_change_batch` | `change_attributes_attribute_change_batch(batch)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
