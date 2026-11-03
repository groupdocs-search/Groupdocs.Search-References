---
title: remove_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes the specified collection of character replacements from this instance of the CharacterReplacementDictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/characterreplacementdictionary/remove_range/
is_root: false
weight: 1060
---


## remove_range {#characters}

Removes the specified collection of character replacements from this instance of the [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/).

```python
def remove_range(self, characters):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| characters | `Iterable[str]` | The collection of characters to remove. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the `IndexStatus.ready` status, or is disposed. |

## remove_range {#code_points}

Removes the specified collection of Unicode code point replacements from this [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/).

```python
def remove_range(self, code_points):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| code_points | `Iterable[int]` | The collection of Unicode code points to remove. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the `IndexStatus.ready` status, or is disposed. |

### Example

```python
from groupdocs.search import Index, IndexSettings

index = Index("./index", IndexSettings(), True)
replacements = index.dictionaries.character_replacements

# Remove the hyphen character replacement
replacements.remove_range([ord("-")])
```

## remove_range {#characters}

Removes the specified collection of character replacements from this instance of the [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/).

```python
def remove_range(self, characters):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| characters | `list[str]` | The collection of characters to remove. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the `IndexStatus.ready` status, or is disposed. |

## remove_range {#code_points}

Removes the specified collection of Unicode code points replacements from this instance of the CharacterReplacementDictionary.

```python
def remove_range(self, code_points):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| code_points | `list[int]` | The collection of Unicode code points to remove. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the Ready status or is disposed. |

### Aliases

These names call `remove_range` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `remove_range_ienumerable` | `remove_range_ienumerable(code_points)`<br>`remove_range_ienumerable(characters)` |
| `remove_range_int32` | `remove_range_int32(code_points)` |
| `remove_range_char` | `remove_range_char(characters)` |

### See Also
* class [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/)
