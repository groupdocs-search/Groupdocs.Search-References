---
title: FileLogger class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a logger that logs events and errors to a local file."
type: docs
url: /python-net/groupdocs.search.common/filelogger/
is_root: false
weight: 140
---


## FileLogger class

Represents a logger that logs events and errors to a local file.

Learn more

- Logging: https://docs.groupdocs.com/search/python-net/logging/

The FileLogger type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.common/filelogger/__init__/#file_path-max_size) | Initializes a new FileLogger instance. |

### Methods
| Method | Description |
| :- | :- |
| [error](/search/python-net/groupdocs.search.common/filelogger/error/#message) | Logs an error that occurred in the index. |
| [trace](/search/python-net/groupdocs.search.common/filelogger/trace/#message) | Logs an event that occurred in the index. |

### Properties
| Property | Description |
| :- | :- |
| [file_path](/search/python-net/groupdocs.search.common/filelogger/file_path/) | The log file path. |
| [max_size](/search/python-net/groupdocs.search.common/filelogger/max_size/) | The maximum size of the log file in megabytes. |

### Example

```python
import os
from groupdocs.search import Index, IndexSettings
from groupdocs.search.common import FileLogger

log_path = "./output/log.txt"
os.makedirs("./output", exist_ok=True)

settings = IndexSettings()
settings.logger = FileLogger(log_path, 4.0)  # path to log file and max size 4 MB

index = Index("./index", settings)
index.add("./documents")
result = index.search("Einstein")

with open(log_path, encoding="utf-8") as f:
    print(f.read())
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
