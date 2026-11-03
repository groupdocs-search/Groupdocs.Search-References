---
title: ILogger class
second_title: GroupDocs.Search for Python via .NET API References
description: "Defines interface of a logger that is used for logging events and errors in an index."
type: docs
url: /python-net/groupdocs.search.common/ilogger/
is_root: false
weight: 200
---


## ILogger class

Defines interface of a logger that is used for logging events and errors in an index.

Learn more:

- Logging (https://docs.groupdocs.com/search/python-net/logging/)

The ILogger type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [error](/search/python-net/groupdocs.search.common/ilogger/error/#message) | Logs an error that occurred in the index. |
| [trace](/search/python-net/groupdocs.search.common/ilogger/trace/#message) | Logs an event that occurred in the index. |

### Example

```python
class ConsoleLogger:
    def error(self, message):
        print("Error: " + message)

    def trace(self, message):
        print(message)
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
