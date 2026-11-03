---
title: error method
second_title: GroupDocs.Search for Python via .NET API References
description: "Logs an error that occurred in the index."
type: docs
url: /python-net/groupdocs.search.common/ilogger/error/
is_root: false
weight: 1010
---


## error {#message}

Logs an error that occurred in the index.

```python
def error(self, message):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| message | `str` | The error message. |

### Example

```python
    class ConsoleLogger:
        def error(self, message):
            print("Error: " + message)

        def trace(self, message):
            print(message)
    ```

### Aliases

These names call `error` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `error_file` | `error_file(message)` |
| `error_string` | `error_string(message)` |

### See Also
* class [`ILogger`](/search/python-net/groupdocs.search.common/ilogger/)
