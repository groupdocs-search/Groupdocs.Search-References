---
title: set_dictionary method
second_title: GroupDocs.Search for Python via .NET API References
description: "Sets a dictionary in the specified shard."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/set_dictionary/
is_root: false
weight: 1180
---


## set_dictionary {#dictionary-shard_index}

Sets a dictionary in the specified shard.

The alphabet, tokenization dictionary, stop word dictionary, and character replacement dictionary define how document text is divided into terms. Therefore a shard accepts a new dictionary only while its index contains no documents and performs no operation. A shard that does not accept the dictionary retains its existing one and writes the reason to its log.

```python
def set_dictionary(self, dictionary, shard_index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| dictionary | `DictionaryBase` | The dictionary. |
| shard_index | `int` | The shard index. |

### Example

```python
from groupdocs.search.dictionaries import CharacterType

# `node` is the master node of a configured and started search network
indexer = node.indexer
shard_index = node.get_shard_indices()[0]

# A shard accepts a tokenization dictionary only while its index holds no documents
dictionary = indexer.get_tokenization_dictionary(shard_index)
dictionary.set_range(list(range(0x3040, 0x30FF + 1)), CharacterType.LETTER)  # Hiragana and Katakana
indexer.set_dictionary(dictionary, shard_index)
```

## set_dictionary {#dictionary}

Sets a dictionary in all shards.

The alphabet, the tokenization dictionary, the stop word dictionary and the character replacement dictionary define how the text of documents is divided into terms. Therefore a shard accepts another content of such a dictionary only while its index contains no documents and performs no operation. A shard that does not accept the dictionary keeps its own one and writes the reason to its log.

```python
def set_dictionary(self, dictionary):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| dictionary | `DictionaryBase` | The dictionary. |

### Example

```python
# Assume `node` is an initialized network node
indexer = node.indexer

# `dictionary` should be a GroupDocs.Search dictionary instance,
# such as a tokenization dictionary created or retrieved earlier.
indexer.set_dictionary(dictionary)
```

### Aliases

These names call `set_dictionary` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `set_dictionary_dictionary_base` | `set_dictionary_dictionary_base(dictionary, shard_index)`<br>`set_dictionary_dictionary_base(dictionary)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
