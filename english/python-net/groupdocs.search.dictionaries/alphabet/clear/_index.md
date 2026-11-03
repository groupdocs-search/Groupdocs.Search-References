---
title: clear method
second_title: GroupDocs.Search for Python via .NET API References
description: "Sets the Separator type for all characters in this Alphabet."
type: docs
url: /python-net/groupdocs.search.dictionaries/alphabet/clear/
is_root: false
weight: 1010
---


## clear

Sets the Separator type for all characters in this Alphabet.

```python
def clear(self):
    ...
```

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the Ready status, or is disposed. |

### Example

```python
# Clear the alphabet of the index's dictionaries
new_index.dictionaries.alphabet.clear()
```

### See Also
* class [`Alphabet`](/search/python-net/groupdocs.search.dictionaries/alphabet/)
