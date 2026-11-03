---
title: add_master_node method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds a node to the search network configuration."
type: docs
url: /python-net/groupdocs.search.scaling.configuring/configurator/add_master_node/
is_root: false
weight: 1010
---


## add_master_node {#node_index}

Adds a node to the search network configuration.

A search network consists of exactly one master node and one or more slave nodes. Each node is identified by a unique non‑negative node index. Use this method to configure the master node, which returns a [`MasterNodeConfigurator`](/search/python-net/groupdocs.search.scaling.configuring/masternodeconfigurator/) for further setup.

```python
def add_master_node(self, node_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| node_index | `int` | The node index. |

**Returns:** MasterNodeConfigurator: The node configurator.

### Example

```python
from groupdocs.search.scaling.configuring import Configurator

config = Configurator()
master = config.add_master_node(0)
# Continue configuring the master node using `master`
```

### Aliases

These names call `add_master_node` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_master_node_int32` | `add_master_node_int32(node_index)` |

### See Also
* class [`Configurator`](/search/python-net/groupdocs.search.scaling.configuring/configurator/)
