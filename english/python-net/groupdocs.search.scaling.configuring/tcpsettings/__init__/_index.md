---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new TcpSettings instance."
type: docs
url: /python-net/groupdocs.search.scaling.configuring/tcpsettings/__init__/
is_root: false
weight: 10
---


## __init__ {#listening_port-send_timeout-receive_timeout-connect_timeout-retry_timeout}

Initializes a new TcpSettings instance.

```python
def __init__(self, listening_port, send_timeout, receive_timeout, connect_timeout, retry_timeout):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| listening_port | `int` | The listening port. |
| send_timeout | `int` | The send timeout in milliseconds. |
| receive_timeout | `int` | The receive timeout in milliseconds. |
| connect_timeout | `int` | The connect timeout in milliseconds. |
| retry_timeout | `int` | The retry timeout in milliseconds. |

### Example

```python
from groupdocs.search.scaling.configuring import TcpSettings

# listening port 49100, timeouts in milliseconds
tcp_settings = TcpSettings(49100, 3000, 3000, 3000, 1000)
```

### See Also
* class [`TcpSettings`](/search/python-net/groupdocs.search.scaling.configuring/tcpsettings/)
