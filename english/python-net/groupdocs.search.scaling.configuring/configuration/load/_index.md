---
title: load method
second_title: GroupDocs.Search for Python via .NET API References
description: "Loads a search network configuration from a file."
type: docs
url: /python-net/groupdocs.search.scaling.configuring/configuration/load/
is_root: false
weight: 1010
---


## load {#file_path}

Loads a search network configuration from a file.

```python
def load(cls, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| file_path | `str` | The file to load from. |

**Returns:** The configuration.

### Example

```python
from groupdocs.search.scaling.configuring import Configuration

base_path = "./SearchNetwork/"
configuration = Configuration.load(base_path + "Configuration.xml")
```

## load {#stream}

Loads a search network configuration from a stream.

```python
def load(cls, stream):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| stream | `io.RawIOBase` | The stream to load from. |

**Returns:** Configuration: The configuration.

### Aliases

These names call `load` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `load_file` | `load_file(file_path)` |
| `load_string` | `load_string(file_path)` |
| `load_stream` | `load_stream(stream)` |
| `load_streams` | `load_streams(stream)` |

### See Also
* class [`Configuration`](/search/python-net/groupdocs.search.scaling.configuring/configuration/)
