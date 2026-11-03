---
title: add_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds the specified collection of synonym groups to this SynonymDictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/synonymdictionary/add_range/
is_root: false
weight: 1010
---


## add_range {#synonyms}

Adds the specified collection of synonym groups to this SynonymDictionary.

```python
def add_range(self, synonyms):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| synonyms | `Iterable[list[str]]` | The collection of synonym groups to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `ValueError` | Raised when number of synonyms in a group is less than 2. |

### Example

```python
synonym_groups = [
    ["achieve", "accomplish", "attain", "reach"],
    ["accept", "take", "have"],
]
synonyms.add_range(synonym_groups)
print("Words in the dictionary:", synonyms.count)
```

### Aliases

These names call `add_range` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_range_files` | `add_range_files(synonyms)` |
| `add_range_strings` | `add_range_strings(synonyms)` |
| `add_range_ienumerable` | `add_range_ienumerable(synonyms)` |

### See Also
* class [`SynonymDictionary`](/search/python-net/groupdocs.search.dictionaries/synonymdictionary/)
