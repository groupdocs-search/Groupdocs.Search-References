---
title: get_dictionary method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets a dictionary from the specified shard."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/get_dictionary/
is_root: false
weight: 1100
---


## get_dictionary {#dictionary_type-shard_index}

Gets a dictionary from the specified shard.

```python
def get_dictionary(self, dictionary_type, shard_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| dictionary_type | `DictionaryType` | The dictionary type. |
| shard_index | `int` | The shard index. |

**Returns:** The dictionary.

### Example

```python
from groupdocs.search.dictionaries import DictionaryType

# `node` is the master node of a configured and started search network
indexer = node.indexer

# Get the stop word dictionary of the first shard
shard_index = node.get_shard_indices()[0]
dictionary = indexer.get_dictionary(DictionaryType.STOP_WORD_DICTIONARY, shard_index)
```

### Aliases

These names call `get_dictionary` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_dictionary_dictionary_type` | `get_dictionary_dictionary_type(dictionary_type, shard_index)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
