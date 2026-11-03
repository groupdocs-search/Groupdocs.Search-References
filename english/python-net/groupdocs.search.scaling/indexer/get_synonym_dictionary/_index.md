---
title: get_synonym_dictionary method
second_title: GroupDocs.Search for Python via .NET API References
description: "Retrieves the synonym dictionary."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/get_synonym_dictionary/
is_root: false
weight: 1150
---


## get_synonym_dictionary {#shard_index}

Retrieves the synonym dictionary.

Obtains the synonym dictionary for the specified shard.

```python
def get_synonym_dictionary(self, shard_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| shard_index | `int` | The shard index. |

**Returns:** The dictionary.

### Example

```python
indices = node.get_shard_indices()
dictionary = indexer.get_synonym_dictionary(indices[0])
if clear_before_adding:
    dictionary.clear()
```

### Aliases

These names call `get_synonym_dictionary` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_synonym_dictionary_int32` | `get_synonym_dictionary_int32(shard_index)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
