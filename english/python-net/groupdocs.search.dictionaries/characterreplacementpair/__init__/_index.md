---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new CharacterReplacementPair."
type: docs
url: /python-net/groupdocs.search.dictionaries/characterreplacementpair/__init__/
is_root: false
weight: 10
---


## __init__ {#character-replacement}

Initializes a new CharacterReplacementPair.

```python
def __init__(self, character, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| character | `str` | The character to be replaced. |
| replacement | `str` | The replacement. |

### Example

```python
from groupdocs.search.dictionaries import CharacterReplacementPair

pairs = [
    CharacterReplacementPair("Ä", "a"),
    CharacterReplacementPair("ä", "a"),
    CharacterReplacementPair(0x1D400, 0x0061),  # Mathematical bold capital A → 'a'
]
```

## __init__ {#character-replacement}

Initializes a new CharacterReplacementPair.

```python
def __init__(self, character, replacement):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| character | `int` | The Unicode code point to be replaced. |
| replacement | `int` | The replacement Unicode code point. |

### Example

```python
from groupdocs.search.dictionaries import CharacterReplacementPair

# Adding character replacements to a dictionary
pairs = [
    CharacterReplacementPair("Ä", "a"),
    CharacterReplacementPair("ä", "a"),
    CharacterReplacementPair(0x1D400, 0x0061),  # Mathematical bold capital A → 'a'
]
replacements.add_range(pairs)

# Creating replacements for all lowercase characters
character_replacements = []
for code_point in range(0x10000):
    character = chr(code_point)
    repl = character.lower()
    if repl != character and len(repl) == 1:
        character_replacements.append(CharacterReplacementPair(character, repl))
```

### See Also
* class [`CharacterReplacementPair`](/search/python-net/groupdocs.search.dictionaries/characterreplacementpair/)
