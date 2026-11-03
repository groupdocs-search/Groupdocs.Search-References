---
title: contains method
second_title: GroupDocs.Search for Python via .NET API References
description: "Determines whether the AliasDictionary contains the specified alias."
type: docs
url: /python-net/groupdocs.search.dictionaries/aliasdictionary/contains/
is_root: false
weight: 1050
---


## contains {#alias}

Determines whether the AliasDictionary contains the specified alias.

```python
def contains(self, alias):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| alias | `str` | The alias to locate in the AliasDictionary. |

**Returns:** bool: True if the AliasDictionary contains the specified alias; otherwise, False.

| Raises | Description |
| :- | :- |
| `ValueError` | When `alias` is None. |

### Example

```python
if aliases.contains("e"):
    replacement = aliases.get_text("e")
```

### Aliases

These names call `contains` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `contains_file` | `contains_file(alias)` |
| `contains_string` | `contains_string(alias)` |

### See Also
* class [`AliasDictionary`](/search/python-net/groupdocs.search.dictionaries/aliasdictionary/)
