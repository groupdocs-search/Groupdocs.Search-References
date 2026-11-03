---
title: clear method
second_title: GroupDocs.Search for Python via .NET API References
description: "Removes all words from a SpellingCorrector object."
type: docs
url: /python-net/groupdocs.search.dictionaries/spellingcorrector/clear/
is_root: false
weight: 1020
---


## clear

Removes all words from a [`SpellingCorrector`](/search/python-net/groupdocs.search.dictionaries/spellingcorrector/) object.

```python
def clear(self):
    ...
```

### Example

```python
from groupdocs.search import Index

index = Index("./index")
corrector = index.dictionaries.spelling_corrector
if corrector.count > 0:
    # Removing all words from the dictionary
    corrector.clear()
```

### See Also
* class [`SpellingCorrector`](/search/python-net/groupdocs.search.dictionaries/spellingcorrector/)
