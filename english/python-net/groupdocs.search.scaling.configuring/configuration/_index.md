---
title: Configuration class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a search network configuration."
type: docs
url: /python-net/groupdocs.search.scaling.configuring/configuration/
is_root: false
weight: 10
---


## Configuration class

Represents a search network configuration.

The Configuration type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [load](/search/python-net/groupdocs.search.scaling.configuring/configuration/load/#file_path) | Loads a search network configuration from a file. |
| [load](/search/python-net/groupdocs.search.scaling.configuring/configuration/load/#stream) | Loads a search network configuration from a stream. |
| [save](/search/python-net/groupdocs.search.scaling.configuring/configuration/save/#file_path) | Saves this configuration to a file. |
| [save](/search/python-net/groupdocs.search.scaling.configuring/configuration/save/#stream) | Saves this configuration to a stream. |

### Example

```python
import os
from groupdocs.search.scaling.configuring import Configuration

base_path = "./SearchNetwork/"
os.makedirs(base_path, exist_ok=True)

# Assume `config` is a Configuration instance configured as needed
config.save(os.path.join(base_path, "Configuration.xml"))

# Load the saved configuration
loaded_config = Configuration.load(os.path.join(base_path, "Configuration.xml"))
```

### See Also
* module [`groupdocs.search.scaling.configuring`](/search/python-net/groupdocs.search.scaling.configuring/)
