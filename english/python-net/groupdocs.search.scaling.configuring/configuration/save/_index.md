---
title: save method
second_title: GroupDocs.Search for Python via .NET API References
description: "Saves this configuration to a file."
type: docs
url: /python-net/groupdocs.search.scaling.configuring/configuration/save/
is_root: false
weight: 1020
---


## save {#file_path}

Saves this configuration to a file.

```python
def save(self, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The file to save to. |

### Example

```python
import os

from groupdocs.search.scaling.configuring import Configurator

base_path = "./SearchNetwork/"

configuration = (Configurator()
    .add_master_node(0)
        .add_indexer(base_path + "Indexer0")
        .add_searcher(base_path + "Searcher0")
        .complete_node()
    .add_slave_node(1)
        .set_tcp_endpoint("127.0.0.1", 49101)
        .add_shard(base_path + "Shard1")
        .add_extractor(base_path + "Extractor1")
        .complete_node()
    .complete_configuration())

# The folder must exist
os.makedirs(base_path, exist_ok=True)
configuration.save(base_path + "Configuration.xml")
```

## save {#stream}

Saves this configuration to a stream.

```python
def save(self, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| stream | `io.RawIOBase` | The stream to save to. |

### Example

```python
from groupdocs.search.scaling.configuring import Configurator

base_path = "./SearchNetwork/"

configuration = (Configurator()
    .add_master_node(0)
        .add_indexer(base_path + "Indexer0")
        .add_searcher(base_path + "Searcher0")
        .complete_node()
    .add_slave_node(1)
        .set_tcp_endpoint("127.0.0.1", 49101)
        .add_shard(base_path + "Shard1")
        .add_extractor(base_path + "Extractor1")
        .complete_node()
    .complete_configuration())

with open("Configuration.xml", "wb") as stream:
    configuration.save(stream)
```

### Aliases

These names call `save` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `save_file` | `save_file(file_path)` |
| `save_string` | `save_string(file_path)` |
| `save_stream` | `save_stream(stream)` |
| `save_streams` | `save_streams(stream)` |

### See Also
* class [`Configuration`](/search/python-net/groupdocs.search.scaling.configuring/configuration/)
