---
title: set_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Sets the character type for each character in the specified collection."
type: docs
url: /python-net/groupdocs.search.dictionaries/alphabet/set_range/
is_root: false
weight: 1040
---


## set_range {#characters-type}

Sets the character type for each character in the specified collection.

```python
def set_range(self, characters, type):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| characters | `list[str]` | The collection of characters to set the type for. Can be a list of Unicode code points (int) or strings. |
| type | `CharacterType` | The character type (`CharacterType`). |

| Raises | Description |
| :- | :- |
| `RuntimeError` | If the dictionary belongs to an index that contains documents, is not in the `IndexStatus.ready` status, or has been disposed. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.dictionaries import CharacterType

index = Index("./MyIndex")
# Treat the hyphen and the ampersand as blended characters
index.dictionaries.alphabet.set_range(["-", "&"], CharacterType.BLENDED)
```

## set_range {#characters-type}

Sets the type for each character in the specified collection for this Alphabet instance.

```python
def set_range(self, characters, type):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| characters | `list[str]` | The collection of characters, surrogate pairs, or Unicode code points to set the type. |
| type | `CharacterType` | The character type (`CharacterType`). |

| Raises | Description |
| :- | :- |
| `RuntimeError` | If the dictionary belongs to an index that contains documents, is not in the `IndexStatus.ready` status, or has been disposed. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.dictionaries import CharacterType

index = Index("./MyIndex")
# A character outside the Basic Multilingual Plane is given as a string
index.dictionaries.alphabet.set_range(["\U0001D41A", "\U0001D41B"], CharacterType.LETTER)  # Mathematical bold small a and b
```

## set_range {#code_points-type}

Sets the character type for each Unicode code point in the given collection.

```python
def set_range(self, code_points, type):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| code_points | `list[int]` | The collection of Unicode code points to set the type. |
| type | `CharacterType` | The character type. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the Ready status or is disposed. |

### Example

```python
from groupdocs.search.dictionaries import CharacterType

# Set the type for characters outside the Basic Multilingual Plane
alphabet.set_range([0x1D400, 0x1D401], CharacterType.LETTER)  # Mathematical bold capital A and B
alphabet.set_range(["\U0001D41A"], CharacterType.LETTER)      # Mathematical bold small A
```

### Aliases

These names call `set_range` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `set_range_files` | `set_range_files(characters, type)` |
| `set_range_strings` | `set_range_strings(characters, type)` |
| `set_range_int32` | `set_range_int32(code_points, type)` |
| `set_range_char` | `set_range_char(characters, type)` |

### See Also
* class [`Alphabet`](/search/python-net/groupdocs.search.dictionaries/alphabet/)
