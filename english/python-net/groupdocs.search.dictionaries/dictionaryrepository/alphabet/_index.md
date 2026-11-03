---
title: alphabet property
second_title: GroupDocs.Search for Python via .NET API References
description: "The dictionary of characters used by the internal tokenization mechanism to split text into words."
type: docs
url: /python-net/groupdocs.search.dictionaries/dictionaryrepository/alphabet/
is_root: false
weight: 2020
---


## alphabet property

The dictionary of characters used by the internal tokenization mechanism to split text into words.

The dictionary defines how the text of documents is divided into terms, so it can be changed only while the index contains no documents and its status is `IndexStatus.ready`.

### Definition:
```python
@property
def alphabet(self):
    ...
```

### See Also
* class [`DictionaryRepository`](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/)
