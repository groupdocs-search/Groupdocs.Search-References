---
title: SearchNetworkNode class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a search network node that can contain services such as extractor, indexer, searcher, and shard."
type: docs
url: /python-net/groupdocs.search.scaling/searchnetworknode/
is_root: false
weight: 20
---


## SearchNetworkNode class

Represents a search network node that can contain services such as extractor, indexer, searcher, and shard.

The SearchNetworkNode type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [configure_all_nodes](/search/python-net/groupdocs.search.scaling/searchnetworknode/configure_all_nodes/) | Configures all nodes in the search network. |
| [configure_node](/search/python-net/groupdocs.search.scaling/searchnetworknode/configure_node/#node_index) | Configures the specified node in the search network. |
| [create_master_node](/search/python-net/groupdocs.search.scaling/searchnetworknode/create_master_node/#node_index-storage_path-network_settings-logger-configuration) | Creates a master node of the search network. |
| [create_slave_node](/search/python-net/groupdocs.search.scaling/searchnetworknode/create_slave_node/#node_index-storage_path-network_settings) | Creates a slave node of the search network. |
| [create_slave_node](/search/python-net/groupdocs.search.scaling/searchnetworknode/create_slave_node/#node_index-storage_path-network_settings-logger) | Creates a slave node of the search network. |
| [dispose](/search/python-net/groupdocs.search.scaling/searchnetworknode/dispose/) | Releases all resources used by the SearchNetworkNode. |
| [get_node_index](/search/python-net/groupdocs.search.scaling/searchnetworknode/get_node_index/#service_index) | Returns the index of the node where the service is located. |
| [get_shard_indices](/search/python-net/groupdocs.search.scaling/searchnetworknode/get_shard_indices/) | Retrieves an array of all shard indices in the search network. |
| [set_ocr_connector](/search/python-net/groupdocs.search.scaling/searchnetworknode/set_ocr_connector/#ocr_connector) | Sets an OCR connector that is used for OCR processing. |
| [set_word_forms_provider](/search/python-net/groupdocs.search.scaling/searchnetworknode/set_word_forms_provider/#word_forms_provider) | Sets a word forms provider. |
| [start](/search/python-net/groupdocs.search.scaling/searchnetworknode/start/) | Starts the functioning of the search network node. |

### Properties
| Property | Description |
| :- | :- |
| [custom_extractors](/search/python-net/groupdocs.search.scaling/searchnetworknode/custom_extractors/) | The custom extractor collection. |
| [events](/search/python-net/groupdocs.search.scaling/searchnetworknode/events/) | The event hub for subscribing to events. |
| [indexer](/search/python-net/groupdocs.search.scaling/searchnetworknode/indexer/) | The indexer. |
| [node_index](/search/python-net/groupdocs.search.scaling/searchnetworknode/node_index/) | The index of the search network node. |
| [searcher](/search/python-net/groupdocs.search.scaling/searchnetworknode/searcher/) | The searcher. |

### Example

```python
from groupdocs.search.scaling import SearchNetworkNode
from groupdocs.search.scaling.configuring import Configuration, TcpSettings
from groupdocs.search.common import FileLogger

base_path = "./SearchNetwork/"
base_port = 49100

# Create and start the master node
master = SearchNetworkNode.create_master_node(
    0,
    base_path + "Node0",
    TcpSettings(base_port, 3000, 3000, 3000, 1000),
    FileLogger(base_path + "Log.txt", 4.0),
    Configuration.load(base_path + "Configuration.xml")
)
master.configure_all_nodes()
master.start()

# Stop the node when done
input("Press Enter to stop the master node\n")
master.dispose()
```

### See Also
* module [`groupdocs.search.scaling`](/search/python-net/groupdocs.search.scaling/)
