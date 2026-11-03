---
title: document_filter property
second_title: GroupDocs.Search for Python via .NET API References
description: "The document filter applied during indexing; when None, all added documents are indexed."
type: docs
url: /python-net/groupdocs.search/indexsettings/document_filter/
is_root: false
weight: 2020
---


## document_filter property

The document filter applied during indexing; when `None`, all added documents are indexed.

The filter works on inclusion logic. Use the [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/) class to create filter instances. The value can be changed at any time. A change made after an index was created is saved in the index by the next operation that modifies the index.

### Definition:
```python
@property
def document_filter(self):
    ...
@document_filter.setter
def document_filter(self, value):
    ...
```

### See Also
* class [`IndexSettings`](/search/python-net/groupdocs.search/indexsettings/)
