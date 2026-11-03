---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new SimilarityLevel instance."
type: docs
url: /python-net/groupdocs.search.options/similaritylevel/__init__/
is_root: false
weight: 10
---


## __init__ {#value}

Initializes a new SimilarityLevel instance.

```python
def __init__(self, value):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| value | `float` | The similarity level value. |

### Example

```python
from groupdocs.search.options import SimilarityLevel

# Create a similarity level with strictness 0.8 (0.0 = loose, 1.0 = strict)
level = SimilarityLevel(0.8)
```

### See Also
* class [`SimilarityLevel`](/search/python-net/groupdocs.search.options/similaritylevel/)
