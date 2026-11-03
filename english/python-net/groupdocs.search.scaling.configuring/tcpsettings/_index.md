---
title: TcpSettings class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents TCP network settings."
type: docs
url: /python-net/groupdocs.search.scaling.configuring/tcpsettings/
is_root: false
weight: 80
---


## TcpSettings class

Represents TCP network settings.

The TcpSettings type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.scaling.configuring/tcpsettings/__init__/#listening_port-send_timeout-receive_timeout-connect_timeout-retry_timeout) | Initializes a new TcpSettings instance. |

### Properties
| Property | Description |
| :- | :- |
| [connect_timeout](/search/python-net/groupdocs.search.scaling.configuring/tcpsettings/connect_timeout/) | The connect timeout in milliseconds. |
| [listening_port](/search/python-net/groupdocs.search.scaling.configuring/tcpsettings/listening_port/) | The listening port. |
| [receive_timeout](/search/python-net/groupdocs.search.scaling.configuring/tcpsettings/receive_timeout/) | The receive timeout in milliseconds. |
| [retry_timeout](/search/python-net/groupdocs.search.scaling.configuring/tcpsettings/retry_timeout/) | The retry timeout in milliseconds. |
| [send_timeout](/search/python-net/groupdocs.search.scaling.configuring/tcpsettings/send_timeout/) | The send timeout in milliseconds. |

### Example

```python
from groupdocs.search.scaling.configuring import TcpSettings

# base_port is the starting port number for the master node
settings = TcpSettings(base_port, 3000, 3000, 3000, 1000)
```

### See Also
* module [`groupdocs.search.scaling.configuring`](/search/python-net/groupdocs.search.scaling.configuring/)
