---
title: configure_all_nodes method
second_title: GroupDocs.Search for Python via .NET API References
description: "Configures all nodes in the search network."
type: docs
url: /python-net/groupdocs.search.scaling/searchnetworknode/configure_all_nodes/
is_root: false
weight: 1010
---


## configure_all_nodes

Configures all nodes in the search network.

```python
def configure_all_nodes(self):
    ...
```

### Example

```python
from groupdocs.search.common import FileLogger
from groupdocs.search.scaling import SearchNetworkNode
from groupdocs.search.scaling.configuring import Configuration, TcpSettings

base_path = "./SearchNetwork/"
base_port = 49100
configuration = Configuration.load(base_path + "Configuration.xml")

# Start the slave nodes first: configure_all_nodes waits until every one of them accepts the connection
node = SearchNetworkNode.create_master_node(
    0,
    base_path + "Node0",
    TcpSettings(base_port, 3000, 3000, 3000, 1000),
    FileLogger(base_path + "Log.txt", 4.0),
    configuration,
)
node.configure_all_nodes()
node.start()
```

### See Also
* class [`SearchNetworkNode`](/search/python-net/groupdocs.search.scaling/searchnetworknode/)
