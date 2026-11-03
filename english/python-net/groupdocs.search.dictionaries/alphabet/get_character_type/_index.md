---
title: get_character_type method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets the type of a character."
type: docs
url: /python-net/groupdocs.search.dictionaries/alphabet/get_character_type/
is_root: false
weight: 1020
---


## get_character_type {#character}

Gets the type of a character.

```python
def get_character_type(self, character):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| character | `str` | The character whose type is to be retrieved. |

**Returns:** The type of the character.

### Example

```python
from groupdocs.search.dictionaries import CharacterType

# Get character type by Unicode code point
type1 = alphabet.get_character_type(0x1D400)
print(type1.name)

# Get character type by string character
type2 = alphabet.get_character_type("\U0001D41A")
print(type2.name)

# Example with hyphen
hyphen_type = alphabet.get_character_type("-")
print(hyphen_type.name)
if hyphen_type != CharacterType.BLENDED:
    alphabet.set_range(["-"], CharacterType.BLENDED)
```

## get_character_type {#code_point}

Gets the type of a Unicode code point.

```python
def get_character_type(self, code_point):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| code_point | `int` | The Unicode code point to get a type. |

**Returns:** The type of the Unicode code point.

### Example

```python
# Assume `alphabet` is an instance of Alphabet
print("The type of U+1D400:", alphabet.get_character_type(0x1D400).name)
print("The type of U+1D41A:", alphabet.get_character_type("\U0001D41A").name)
```

## get_character_type {#character}

Gets the type of a character.

This method can be used to obtain the type of a surrogate pair.

```python
def get_character_type(self, character):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| character | `str` | The character or surrogate pair to get a type. |

**Returns:** The type of the character.

### Example

```python
# Assume `alphabet` is an instance of `Alphabet`
print("The type of U+1D400:", alphabet.get_character_type(0x1D400).name)
print("The type of U+1D41A:", alphabet.get_character_type("\U0001D41A").name)

# Getting the type of a hyphen character
hyphen_type = alphabet.get_character_type("-")
print("The type of hyphen:", hyphen_type.name)
```

### Aliases

These names call `get_character_type` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_character_type_int32` | `get_character_type_int32(code_point)` |
| `get_character_type_file` | `get_character_type_file(character)` |
| `get_character_type_string` | `get_character_type_string(character)` |
| `get_character_type_char` | `get_character_type_char(character)` |

### See Also
* class [`Alphabet`](/search/python-net/groupdocs.search.dictionaries/alphabet/)
