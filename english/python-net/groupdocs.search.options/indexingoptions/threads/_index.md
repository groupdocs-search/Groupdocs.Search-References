---
title: threads property
second_title: GroupDocs.Search for Python via .NET API References
description: "The number of threads used for indexing (default is 1, must be between 1 and 4)."
type: docs
url: /python-net/groupdocs.search.options/indexingoptions/threads/
is_root: false
weight: 2040
---


## threads property

The number of threads used for indexing (default is 1, must be between 1 and 4).

The threads property is used to set the number of threads used for indexing. The default value is 1. The number of indexing threads cannot be less than 1 or more than 4. A larger number of threads accelerates the indexing process.

### Definition:
```python
@property
def threads(self):
    ...
@threads.setter
def threads(self, value):
    ...
```

### See Also
* class [`IndexingOptions`](/search/python-net/groupdocs.search.options/indexingoptions/)
