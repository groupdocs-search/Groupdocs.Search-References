---
title: get_homophones method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets the homophones for the specified word."
type: docs
url: /python-net/groupdocs.search.dictionaries/homophonedictionary/get_homophones/
is_root: false
weight: 1060
---


## get_homophones {#word}

Gets the homophones for the specified word.

The case of the letters of the word is not taken into account.

```python
def get_homophones(self, word):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| word | `str` | The word to suggest the homophones. |

**Returns:** The homophones for the specified word or empty list if the HomophoneDictionary object does not contain the specified word.

| Raises | Description |
| :- | :- |
| `ValueError` | When `word` is None. |

### Example

```python
words = homophones.get_homophones("Braid")
print("Homophones for 'braid':")
for w in words:
    print(w)
```

### Aliases

These names call `get_homophones` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_homophones_file` | `get_homophones_file(word)` |
| `get_homophones_string` | `get_homophones_string(word)` |

### See Also
* class [`HomophoneDictionary`](/search/python-net/groupdocs.search.dictionaries/homophonedictionary/)
