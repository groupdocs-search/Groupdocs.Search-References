---
title: clear method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes all character replacements from the dictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/characterreplacementdictionary/clear/
is_root: false
weight: 1020
---


## clear

Removes all character replacements from the dictionary.

```python
def clear(self):
    ...
```

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the `IndexStatus.ready` status or is disposed. |

### Example

```python
# Delete all character replacements from the index's dictionary
index.dictionaries.character_replacements.clear()
```

### See Also
* class [`CharacterReplacementDictionary`](/search/python-net/groupdocs.search.dictionaries/characterreplacementdictionary/)
