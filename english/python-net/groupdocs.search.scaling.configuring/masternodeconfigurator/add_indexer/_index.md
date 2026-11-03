---
title: add_indexer method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds an indexer service to the search network node."
type: docs
url: /python-net/groupdocs.search.scaling.configuring/masternodeconfigurator/add_indexer/
is_root: false
weight: 1010
---


## add_indexer {#storage_path}

Adds an indexer service to the search network node.

```python
def add_indexer(self, storage_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| storage_path | `str` | The storage path of the adding service. |

**Returns:** MasterNodeConfigurator: This search network node configurator.

### Example

```python
# Configure the master node and add an indexer service
master = search_network.add_master_node(node_index=0)
master.add_indexer(storagePath="/data/indexer")
```

### Aliases

These names call `add_indexer` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_indexer_file` | `add_indexer_file(storage_path)` |
| `add_indexer_string` | `add_indexer_string(storage_path)` |

### See Also
* class [`MasterNodeConfigurator`](/search/python-net/groupdocs.search.scaling.configuring/masternodeconfigurator/)
