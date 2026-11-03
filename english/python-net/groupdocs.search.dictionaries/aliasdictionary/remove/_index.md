---
title: remove method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes the specified alias from an AliasDictionary object."
type: docs
url: /python-net/groupdocs.search.dictionaries/aliasdictionary/remove/
is_root: false
weight: 1080
---


## remove {#alias}

Removes the specified alias from an [`AliasDictionary`](/search/python-net/groupdocs.search.dictionaries/aliasdictionary/) object.

```python
def remove(self, alias):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| alias | `str` | The alias to remove. |

**Returns:** bool: True if the alias is successfully found and removed. False if the alias is not found in the `AliasDictionary` object.

| Raises | Description |
| :- | :- |
| `ValueError` | When `alias` is None. |

### Aliases

These names call `remove` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `remove_file` | `remove_file(alias)` |
| `remove_string` | `remove_string(alias)` |

### See Also
* class [`AliasDictionary`](/search/python-net/groupdocs.search.dictionaries/aliasdictionary/)
