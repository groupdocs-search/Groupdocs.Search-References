---
title: add_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds the specified collection of words to this SpellingCorrector instance."
type: docs
url: /python-net/groupdocs.search.dictionaries/spellingcorrector/add_range/
is_root: false
weight: 1010
---


## add_range {#words}

Adds the specified collection of words to this SpellingCorrector instance.

```python
def add_range(self, words):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| words | `Iterable[str]` | The collection of words to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `ValueError` | When `words` is None. |

### Example

```python
words = ["achieve", "accomplish", "attain", "reach"]
corrector.add_range(words)
```

## add_range {#words}

Adds the specified collection of words to this SpellingCorrector instance.

```python
def add_range(self, words):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| words | `list[str]` | The collection of words to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `ValueError` | If `words` is None. |

### Example

```python
words = ["achieve", "accomplish", "attain", "reach"]
corrector.add_range(words)
```

### Aliases

These names call `add_range` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_range_files` | `add_range_files(words)`<br>`add_range_files(words)` |
| `add_range_strings` | `add_range_strings(words)`<br>`add_range_strings(words)` |
| `add_range_ienumerable` | `add_range_ienumerable(words)` |

### See Also
* class [`SpellingCorrector`](/search/python-net/groupdocs.search.dictionaries/spellingcorrector/)
