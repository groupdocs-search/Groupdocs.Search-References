---
title: add_range method
second_title: GroupDocs.Search for Python via .NET API References
description: "Adds the specified collection of homophone groups to this instance of the HomophoneDictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/homophonedictionary/add_range/
is_root: false
weight: 1010
---


## add_range {#homophones}

Adds the specified collection of homophone groups to this instance of the HomophoneDictionary.

```python
def add_range(self, homophones):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| homophones | `Iterable[list[str]]` | The collection of homophone groups to add to the dictionary. |

| Raises | Description |
| :- | :- |
| `ValueError` | If a group contains fewer than 2 homophones. |

### Example

```python
homophone_groups = [
    ["awe", "oar", "or", "ore"],
    ["aye", "eye", "i"],
]
homophones.add_range(homophone_groups)
print("Words in the dictionary:", homophones.count)
```

### Aliases

These names call `add_range` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_range_files` | `add_range_files(homophones)` |
| `add_range_strings` | `add_range_strings(homophones)` |
| `add_range_ienumerable` | `add_range_ienumerable(homophones)` |

### See Also
* class [`HomophoneDictionary`](/search/python-net/groupdocs.search.dictionaries/homophonedictionary/)
