---
title: get_replacement method
second_title: GroupDocs.Search for Python via .NET API References
description: "Returns the replacement for the specified Unicode code point."
type: docs
url: /python-net/groupdocs.search.dictionaries/characterreplacementdictionary/get_replacement/
is_root: false
weight: 1050
---


## get_replacement {#code_point}

Returns the replacement for the specified Unicode code point.

```python
def get_replacement(self, code_point):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| code_point | `int` | The character to get a replacement for. |

**Returns:** int: The replacement for the specified Unicode code point.

### Example

```python
    # Assuming `replacements` is a CharacterReplacementDictionary instance
    if replacements.contains(ord("-")):
        replacement = replacements.get_replacement(ord("-"))
        print("The replacement for hyphen is " + chr(replacement))
    ```

### Aliases

These names call `get_replacement` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_replacement_int32` | `get_replacement_int32(code_point)` |

### See Also
* class [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/)
