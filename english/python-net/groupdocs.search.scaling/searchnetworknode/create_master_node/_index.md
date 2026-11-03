---
title: create_master_node method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a master node of the search network."
type: docs
url: /python-net/groupdocs.search.scaling/searchnetworknode/create_master_node/
is_root: false
weight: 1030
---


## create_master_node {#node_index-storage_path-network_settings-logger-configuration}

Creates a master node of the search network.

```python
def create_master_node(cls, node_index, storage_path, network_settings, logger, configuration):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| node_index | `int` | The node index. |
| storage_path | `str` | The storage path. |
| network_settings | `INetworkSettings` | The network settings. |
| logger | `ILogger` | The logger. |
| configuration | `Configuration` | The configuration. |

**Returns:** SearchNetworkNode: The master node.

### Example

```python
from groupdocs.search.scaling import SearchNetworkNode
from groupdocs.search.common import FileLogger
from groupdocs.search.scaling.configuring import TcpSettings

node = SearchNetworkNode.create_master_node(
    0,
    "/data/Node0",
    TcpSettings(base_port, 3000, 3000, 3000, 1000),
    FileLogger("/data/Log.txt", 4.0),
    configuration,
)
node.configure_all_nodes()
node.start()
```

### See Also
* class [`SearchNetworkNode`](/search/python-net/groupdocs.search.scaling/searchnetworknode/)
