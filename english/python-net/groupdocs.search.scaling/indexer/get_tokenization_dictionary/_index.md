---
title: get_tokenization_dictionary method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets the tokenization dictionary."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/get_tokenization_dictionary/
is_root: false
weight: 1160
---


## get_tokenization_dictionary {#shard_index}

Gets the tokenization dictionary.

Returns the tokenization dictionary for the specified shard in a search network.

```python
def get_tokenization_dictionary(self, shard_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| shard_index | `int` | The shard index. |

**Returns:** GroupDocs.Search.Scaling.TokenizationDictionary: The dictionary.

### Example

```python
indices = node.get_shard_indices()
token_dict = indexer.get_tokenization_dictionary(indices[0])
```

### Aliases

These names call `get_tokenization_dictionary` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_tokenization_dictionary_int32` | `get_tokenization_dictionary_int32(shard_index)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
