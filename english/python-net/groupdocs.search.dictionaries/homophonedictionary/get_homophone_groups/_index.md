---
title: get_homophone_groups method
second_title: GroupDocs.Search for Python via .NET API References
description: "Returns all groups of homophones to which the specified word belongs."
type: docs
url: /python-net/groupdocs.search.dictionaries/homophonedictionary/get_homophone_groups/
is_root: false
weight: 1050
---


## get_homophone_groups {#word}

Returns all groups of homophones to which the specified word belongs.

The case of the letters of the word is not taken into account: the groups contain the word as the dictionary keeps it, in lower case.

```python
def get_homophone_groups(self, word):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| word | `str` | The word for getting groups of homophones. |

**Returns:** list[list[str]]: All groups of homophones to which the specified word belongs.

| Raises | Description |
| :- | :- |
| `ValueError` | Raised when `word` is None. |

### Example

```python
from groupdocs.search import Index

index = Index("./MyIndex")
homophones = index.dictionaries.homophone_dictionary
groups = homophones.get_homophone_groups("braid")
print("Homophone groups for 'braid':")
for group in groups:
    print(" ".join(group))
if homophones.count > 0:
    # Removing all homophones from the dictionary
    homophones.clear()
```

### Aliases

These names call `get_homophone_groups` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_homophone_groups_file` | `get_homophone_groups_file(word)` |
| `get_homophone_groups_string` | `get_homophone_groups_string(word)` |

### See Also
* class [`HomophoneDictionary`](/search/python-net/groupdocs.search.dictionaries/homophonedictionary/)
