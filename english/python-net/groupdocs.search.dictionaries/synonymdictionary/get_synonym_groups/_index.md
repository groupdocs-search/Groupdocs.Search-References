---
title: get_synonym_groups method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets all groups of synonyms to which the specified word belongs."
type: docs
url: /python-net/groupdocs.search.dictionaries/synonymdictionary/get_synonym_groups/
is_root: false
weight: 1050
---


## get_synonym_groups {#word}

Gets all groups of synonyms to which the specified word belongs.

The case of the letters of the word is not taken into account: the groups contain the word as the dictionary keeps it, in the lower case.

```python
def get_synonym_groups(self, word):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| word | `str` | The word for getting groups of synonyms. |

**Returns:** list[list[str]]: All groups of synonyms to which the specified word belongs.

| Raises | Description |
| :- | :- |
| `ValueError` | If `word` is None. |

### Example

```python
from groupdocs.search import Index

index = Index("./MyIndex")
synonyms = index.dictionaries.synonym_dictionary
groups = synonyms.get_synonym_groups("make")
print("Synonym groups for 'make':")
for group in groups:
    print(" ".join(group))

# Optionally clear the dictionary
if synonyms.count > 0:
    synonyms.clear()
```

### Aliases

These names call `get_synonym_groups` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_synonym_groups_file` | `get_synonym_groups_file(word)` |
| `get_synonym_groups_string` | `get_synonym_groups_string(word)` |

### See Also
* class [`SynonymDictionary`](/search/python-net/groupdocs.search.dictionaries/synonymdictionary/)
