---
title: add_slave_node method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds a node to the search network configuration."
type: docs
url: /python-net/groupdocs.search.scaling.configuring/configurator/add_slave_node/
is_root: false
weight: 1020
---


## add_slave_node {#node_index}

Adds a node to the search network configuration.

```python
def add_slave_node(self, node_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| node_index | `int` | The node index. |

**Returns:** SlaveNodeConfigurator: The node configurator.

### Example

```python
from groupdocs.search.scaling.configuring import Configurator

configurator = Configurator()
slave_node = configurator.add_slave_node(1)
# Use `slave_node` to configure the added slave node.
```

### Aliases

These names call `add_slave_node` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_slave_node_int32` | `add_slave_node_int32(node_index)` |

### See Also
* class [`Configurator`](/search/python-net/groupdocs.search.scaling.configuring/configurator/)
