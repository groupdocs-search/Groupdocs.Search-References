---
title: load_into_memory_completely method
second_title: GroupDocs.Search for Python via .NET API References
description: "Loads the entire index into memory."
type: docs
url: /python-net/groupdocs.search/index/load_into_memory_completely/
is_root: false
weight: 1150
---


## load_into_memory_completely {#index_folder}

Loads the entire index into memory.

Any changes to the index are not automatically saved to the original folder.

```python
def load_into_memory_completely(cls, index_folder):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The index folder path. |

**Returns:** Index: The loaded in-memory index.

## load_into_memory_completely {#index_folder-settings}

Loads the entire index into memory.

Any changes to the index are not automatically saved to the original folder.

```python
def load_into_memory_completely(cls, index_folder, settings):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index_folder | `str` | The index folder path. |
| settings | `IndexSettings` | The index settings object. |

**Returns:** Index: The loaded in-memory index.

### Example

```python
from groupdocs.search import Index, IndexSettings

settings = IndexSettings()
# configure settings, e.g., logger, as needed
in_memory_index = Index.load_into_memory_completely("./index", settings)
```

### Aliases

These names call `load_into_memory_completely` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `load_into_memory_completely_file` | `load_into_memory_completely_file(index_folder, settings)`<br>`load_into_memory_completely_file(index_folder)` |
| `load_into_memory_completely_string` | `load_into_memory_completely_string(index_folder, settings)`<br>`load_into_memory_completely_string(index_folder)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
