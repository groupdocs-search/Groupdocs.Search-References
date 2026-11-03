---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new DocumentField."
type: docs
url: /python-net/groupdocs.search.common/documentfield/__init__/
is_root: false
weight: 10
---


## __init__ {#name-value}

Initializes a new DocumentField.

```python
def __init__(self, name, value):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| name | `str` | The field name. |
| value | `str` | The field value. |

### Example

```python
from groupdocs.search.common import DocumentField

# Create a field containing the file name
field = DocumentField("FileName", "/path/to/file.txt")
```

### See Also
* class [`DocumentField`](/search/python-net/groupdocs.search.common/documentfield/)
