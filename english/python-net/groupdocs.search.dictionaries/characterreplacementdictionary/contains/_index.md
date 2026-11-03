---
title: contains method
second_title: GroupDocs.Search for Python via .NET API References
description: "Determines whether a CharacterReplacementDictionary object contains a replacement for the specified Unicode code point."
type: docs
url: /python-net/groupdocs.search.dictionaries/characterreplacementdictionary/contains/
is_root: false
weight: 1030
---


## contains {#code_point}

Determines whether a [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/) object contains a replacement for the specified Unicode code point.

```python
def contains(self, code_point):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| code_point | `int` | The Unicode code point to locate in the `CharacterReplacementDictionary` object. |

**Returns:** bool: `True` if the `CharacterReplacementDictionary` object contains the specified Unicode code point; otherwise, `False`.

### Example

```python
from groupdocs.search import Index, IndexSettings

# Initialize an index (assumes the index folder is empty)
index = Index("./index", IndexSettings(), True)

# Access the character replacement dictionary
replacements = index.dictionaries.character_replacements

# Check if a replacement for the hyphen character exists
if replacements.contains(ord("-")):
    # Retrieve the replacement for the hyphen character
    replacement = replacements.get_replacement(ord("-"))
    print("The replacement for hyphen is " + chr(replacement))
```

### Aliases

These names call `contains` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `contains_int32` | `contains_int32(code_point)` |

### See Also
* class [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/)
