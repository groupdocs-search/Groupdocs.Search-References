---
title: remove_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes the specified collection of words from this StopWordDictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/stopworddictionary/remove_range/
is_root: false
weight: 1050
---


## remove_range {#words}

Removes the specified collection of words from this StopWordDictionary.

A word is removed as it is added: without surrounding whitespace and in lower case.

```python
def remove_range(self, words):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| words | `Iterable[str]` | The collection of words to remove. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the `IndexStatus.ready` status, or is disposed. |

### Example

```python
# Assume `stop_words` is an instance of StopWordDictionary
if stop_words.contains("But") and stop_words.contains("BY"):
    # Remove the words (case-insensitive)
    stop_words.remove_range(["but", "by"])
```

## remove_range {#words}

Removes the specified collection of words from this StopWordDictionary.

A word is removed as it is added: without surrounding whitespace and in lower case.

```python
def remove_range(self, words):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| words | `list[str]` | The collection of words to remove. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the Ready status or is disposed. |

### Example

```python
    # Assuming `stop_words` is an instance of StopWordDictionary
    if stop_words.contains("But") and stop_words.contains("BY"):
        # Remove words from the dictionary
        stop_words.remove_range(["but", "by"])
    ```

### Aliases

These names call `remove_range` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `remove_range_files` | `remove_range_files(words)`<br>`remove_range_files(words)` |
| `remove_range_strings` | `remove_range_strings(words)`<br>`remove_range_strings(words)` |
| `remove_range_ienumerable` | `remove_range_ienumerable(words)` |

### See Also
* class [`StopWordDictionary`](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/)
