---
title: create_slave_node method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a slave node of the search network."
type: docs
url: /python-net/groupdocs.search.scaling/searchnetworknode/create_slave_node/
is_root: false
weight: 1040
---


## create_slave_node {#node_index-storage_path-network_settings}

Creates a slave node of the search network.

```python
def create_slave_node(cls, node_index, storage_path, network_settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| node_index | `int` | The node index. |
| storage_path | `str` | The storage path. |
| network_settings | `INetworkSettings` | The network settings. |

**Returns:** SearchNetworkNode: The slave node.

### Example

```python
from groupdocs.search.scaling import SearchNetworkNode
from groupdocs.search.scaling.configuring import TcpSettings

node = SearchNetworkNode.create_slave_node(
    1,
    "./SearchNetwork/Node1",
    TcpSettings(49101, 3000, 3000, 3000, 1000)
)
```

## create_slave_node {#node_index-storage_path-network_settings-logger}

Creates a slave node of the search network.

```python
def create_slave_node(cls, node_index, storage_path, network_settings, logger):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| node_index | `int` | The node index. |
| storage_path | `str` | The storage path. |
| network_settings | `INetworkSettings` | The network settings. |
| logger | `ILogger` | The logger. |

**Returns:** SearchNetworkNode: The slave node.

### Example

```python
from groupdocs.search.common import FileLogger
from groupdocs.search.scaling import SearchNetworkNode
from groupdocs.search.scaling.configuring import TcpSettings

base_path = "./SearchNetwork/"
base_port = 49100

# The port and timeouts (in milliseconds) of the node, which must match the configuration
node = SearchNetworkNode.create_slave_node(
    1,
    base_path + "Node1",
    TcpSettings(base_port + 1, 3000, 3000, 3000, 1000),
    FileLogger(base_path + "Node1.log", 4.0))
node.start()
```

### Aliases

These names call `create_slave_node` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `create_slave_node_int32` | `create_slave_node_int32(node_index, storage_path, network_settings, logger)`<br>`create_slave_node_int32(node_index, storage_path, network_settings)` |
| `create_slave_node_file` | `create_slave_node_file(node_index, storage_path, network_settings, logger)`<br>`create_slave_node_file(node_index, storage_path, network_settings)` |
| `create_slave_node_string` | `create_slave_node_string(node_index, storage_path, network_settings, logger)`<br>`create_slave_node_string(node_index, storage_path, network_settings)` |

### See Also
* class [`SearchNetworkNode`](/search/python-net/groupdocs.search.scaling/searchnetworknode/)
