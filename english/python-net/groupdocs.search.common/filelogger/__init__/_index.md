---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new FileLogger instance."
type: docs
url: /python-net/groupdocs.search.common/filelogger/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path-max_size}

Initializes a new FileLogger instance.

```python
def __init__(self, file_path, max_size):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The log file path. |
| max_size | `float` | The maximum size of the log file in megabytes. Must be in the range from 0.1 to 1000. |

### Example

```python
from groupdocs.search.common import FileLogger

log_path = "./output/log.txt"
logger = FileLogger(log_path, 4.0)  # 4 MB max size
```

### See Also
* class [`FileLogger`](/search/python-net/groupdocs.search.common/filelogger/)
