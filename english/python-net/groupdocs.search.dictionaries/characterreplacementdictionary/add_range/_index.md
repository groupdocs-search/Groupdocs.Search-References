---
title: add_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds the specified collection of character replacements to this CharacterReplacementDictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/characterreplacementdictionary/add_range/
is_root: false
weight: 1010
---


## add_range {#character_replacements}

Adds the specified collection of character replacements to this [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/).

```python
def add_range(self, character_replacements):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| character_replacements | `Iterable[KeyValuePair[str, str]]` | The collection of character replacements to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the `IndexStatus.ready` status, or is disposed. |

### Example

```python
from groupdocs.search import Index

index = Index("./MyIndex")
replacements = index.dictionaries.character_replacements

# Each pair is a character and the character that replaces it
replacements.add_range([["Ä", "a"], ["ä", "a"]])
```

## add_range {#character_replacements}

Adds the specified collection of Unicode code point replacements to this instance of the CharacterReplacementDictionary.

From Python, give code points as [`CharacterReplacementPair`](/search/python-net/groupdocs.search.dictionaries/characterreplacementpair/) objects: a list of integer pairs is taken by the overload for characters and fails on a code point above 0xFFFF.

```python
def add_range(self, character_replacements):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| character_replacements | `Iterable[KeyValuePair[int, int]]` | Iterable of Unicode code point replacements to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the Ready status, or is disposed. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.dictionaries import CharacterReplacementPair

index = Index("./MyIndex")
replacements = index.dictionaries.character_replacements

# Each pair is a code point and the code point that replaces it
replacements.add_range([
    CharacterReplacementPair(0x1D400, 0x61),  # Mathematical bold capital A -> a
    CharacterReplacementPair(0x1D41A, 0x61),  # Mathematical bold small a -> a
])
```

## add_range {#character_replacements}

Adds the specified collection of character replacements to this instance of the CharacterReplacementDictionary.

```python
def add_range(self, character_replacements):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| character_replacements | `Iterable[CharacterReplacementPair]` | The collection of character replacements to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the Ready status or is disposed. |

### Example

```python
from groupdocs.search.dictionaries import CharacterReplacementPair

pairs = [
    CharacterReplacementPair("Ä", "a"),
    CharacterReplacementPair("ä", "a"),
    CharacterReplacementPair(0x1D400, 0x0061),  # Mathematical bold capital A → a
]
replacements.add_range(pairs)
```

## add_range {#character_replacements}

Adds the specified collection of character replacements to this instance of the [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/).

```python
def add_range(self, character_replacements):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| character_replacements | `list[CharacterReplacementPair]` | The collection of character replacements to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the `IndexStatus.ready` status, or is disposed. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.dictionaries import CharacterReplacementPair

index = Index("./MyIndex")
replacements = index.dictionaries.character_replacements
replacements.add_range([
    CharacterReplacementPair("Ä", "a"),
    CharacterReplacementPair("ä", "a"),
])
```

### Aliases

These names call `add_range` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_range_ienumerable` | `add_range_ienumerable(character_replacements)`<br>`add_range_ienumerable(character_replacements)`<br>`add_range_ienumerable(character_replacements)` |
| `add_range_character_replacement_pair` | `add_range_character_replacement_pair(character_replacements)` |

### See Also
* class [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/)
