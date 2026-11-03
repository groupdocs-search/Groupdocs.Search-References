---
title: tokenization_dictionary property
second_title: GroupDocs.Search for Python via .NET API References
description: "The dictionary of characters that defines whether a token is considered as a valid word or a separator when using external tokenization tools."
type: docs
url: /python-net/groupdocs.search.dictionaries/dictionaryrepository/tokenization_dictionary/
is_root: false
weight: 2090
---


## tokenization_dictionary property

The dictionary of characters that defines whether a token is considered as a valid word or a separator when using external tokenization tools.

The dictionary defines how the text of documents is divided into terms, so it can be changed only while the index contains no documents and its status is `IndexStatus.ready`.

### Definition:
```python
@property
def tokenization_dictionary(self):
    ...
```

### See Also
* class [`DictionaryRepository`](/search/python-net/groupdocs.search.dictionaries/dictionaryrepository/)
