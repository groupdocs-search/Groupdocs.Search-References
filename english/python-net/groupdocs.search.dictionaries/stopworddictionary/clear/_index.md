---
title: clear method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes all words from the StopWordDictionary."
type: docs
url: /python-net/groupdocs.search.dictionaries/stopworddictionary/clear/
is_root: false
weight: 1020
---


## clear

Removes all words from the StopWordDictionary.

```python
def clear(self):
    ...
```

| Raises | Description |
| :- | :- |
| `RuntimeError` | The call changes the dictionary of an index that contains documents, is not in the Ready status or is disposed. |

### Example

```python
from groupdocs.search import Index, IndexSettings

index = Index("./index", IndexSettings(), True)
stop_words = index.dictionaries.stop_word_dictionary
if stop_words.count > 0:
    stop_words.clear()
```

### See Also
* class [`StopWordDictionary`](/search/python-net/groupdocs.search.dictionaries/stopworddictionary/)
