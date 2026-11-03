---
title: trace method
second_title: GroupDocs.Search for Python via .NET API References
description: "Logs an event that occurred in the index."
type: docs
url: /python-net/groupdocs.search.common/ilogger/trace/
is_root: false
weight: 1020
---


## trace {#message}

Logs an event that occurred in the index.

```python
def trace(self, message):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| message | `str` | The event message. |

### Example

```python
class ConsoleLogger:
    def error(self, message):
        print("Error: " + message)

    def trace(self, message):
        print(message)

logger = ConsoleLogger()
logger.trace("Index built successfully.")
```

### Aliases

These names call `trace` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `trace_file` | `trace_file(message)` |
| `trace_string` | `trace_string(message)` |

### See Also
* class [`ILogger`](/search/python-net/groupdocs.search.common/ilogger/)
