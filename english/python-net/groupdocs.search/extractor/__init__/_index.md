---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new instance of the Extractor class."
type: docs
url: /python-net/groupdocs.search/extractor/__init__/
is_root: false
weight: 10
---


## __init__

Initializes a new instance of the Extractor class.

```python
def __init__(self):
    ...
```

### Example

```python
from groupdocs.search import Extractor

extractor = Extractor()
extractor.error_occurred += lambda sender, args: print(args.message)
```

### See Also
* class [`Extractor`](/search/python-net/groupdocs.search/extractor/)
