---
title: clear method
second_title: GroupDocs.Search for Python via .NET API References
description: "Clears the dictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/dictionarybase/clear/
is_root: false
weight: 1010
---


## clear

Clears the dictionary.

```python
def clear(self):
    ...
```

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes a dictionary that defines how the text of documents is divided into terms (see `DictionaryRepository`), and the index of the dictionary contains documents, is not in the `IndexStatus.ready` status or is disposed. |

### Example

```python
# Clear the alphabet dictionary in an index
index.dictionaries.alphabet.clear()
```

### See Also
* class [`DictionaryBase`](/search/python-net/groupdocs.search.dictionaries/dictionarybase/)
