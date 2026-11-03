---
title: remove method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes the password for the specified document from the dictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/passworddictionary/remove/
is_root: false
weight: 1070
---


## remove {#key}

Removes the password for the specified document from the dictionary.

```python
def remove(self, key):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| key | `str` | The full file path or a document key. |

**Returns:** bool: True if the password was successfully removed; otherwise, False. This method also returns False if the key was not found in the dictionary.

### Aliases

These names call `remove` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `remove_file` | `remove_file(key)` |
| `remove_string` | `remove_string(key)` |

### See Also
* class [`PasswordDictionary`](/search/python-net/groupdocs.search.dictionaries/passworddictionary/)
