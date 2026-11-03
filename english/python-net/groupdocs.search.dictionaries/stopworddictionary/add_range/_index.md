---
title: add_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds the specified collection of words to this StopWordDictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/stopworddictionary/add_range/
is_root: false
weight: 1010
---


## add_range {#words}

Adds the specified collection of words to this StopWordDictionary.

Stop words are excluded from indexing when the `use_stop_words` index setting is enabled.

```python
def add_range(self, words):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| words | `Iterable[str]` | The collection of words to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the `IndexStatus.ready` status, or is disposed. |

### Example

```python
from groupdocs.search import Index

index = Index("./index")
stop_words = index.dictionaries.stop_word_dictionary
stop_words.add_range(["a", "an", "the", "but", "by"])
```

## add_range {#words}

Adds the specified collection of words to the StopWordDictionary instance.

```python
def add_range(self, words):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| words | `list[str]` | The collection of words to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the `IndexStatus.ready` status, or is disposed. |

### Example

```python
# Add stop words to the dictionary of an existing index
index.dictionaries.stop_word_dictionary.add_range(["physics", "chemistry"])
```

### Aliases

These names call `add_range` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_range_files` | `add_range_files(words)`<br>`add_range_files(words)` |
| `add_range_strings` | `add_range_strings(words)`<br>`add_range_strings(words)` |
| `add_range_ienumerable` | `add_range_ienumerable(words)` |

### See Also
* class [`StopWordDictionary`](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/)
