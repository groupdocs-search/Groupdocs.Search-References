---
title: get_synonyms method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets the synonyms for the specified word."
type: docs
url: /python-net/groupdocs.search.dictionaries/synonymdictionary/get_synonyms/
is_root: false
weight: 1060
---


## get_synonyms {#word}

Gets the synonyms for the specified word.

The case of the letters of the word is not taken into account.

```python
def get_synonyms(self, word):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| word | `str` | The word to suggest the synonyms. |

**Returns:** list[str]: The synonyms for the specified word or an empty list if the `SynonymDictionary` object does not contain the specified word.

| Raises | Description |
| :- | :- |
| `ValueError` | When `word` is None. |

### Example

```python
words = synonyms.get_synonyms("Make")
print("Synonyms for 'make':")
for w in words:
    print(w)
```

### Aliases

These names call `get_synonyms` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_synonyms_file` | `get_synonyms_file(word)` |
| `get_synonyms_string` | `get_synonyms_string(word)` |

### See Also
* class [`SynonymDictionary`](/search/python-net/groupdocs.search.dictionaries/synonymdictionary/)
