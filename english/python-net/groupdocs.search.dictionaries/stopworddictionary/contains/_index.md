---
title: contains method
second_title: GroupDocs.Search for Python via .NET API References
description: "Determines whether the StopWordDictionary contains the specified word."
type: docs
url: /python-net/groupdocs.search.dictionaries/stopworddictionary/contains/
is_root: false
weight: 1030
---


## contains {#word}

Determines whether the StopWordDictionary contains the specified word.

The case of the letters of the word is not taken into account.

```python
def contains(self, word):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| word | `str` | The word to locate in the StopWordDictionary. |

**Returns:** bool: True if the StopWordDictionary contains the specified word; otherwise, False.

### Example

```python
if stop_words.contains("But") and stop_words.contains("BY"):
    # Removing words from the dictionary
    stop_words.remove_range(["but", "by"])
```

### Aliases

These names call `contains` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `contains_file` | `contains_file(word)` |
| `contains_string` | `contains_string(word)` |

### See Also
* class [`StopWordDictionary`](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/)
