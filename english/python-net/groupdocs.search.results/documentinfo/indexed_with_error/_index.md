---
title: indexed_with_error property
second_title: GroupDocs.Search for Python via .NET API References
description: "The indicator of indexing error."
type: docs
url: /python-net/groupdocs.search.results/documentinfo/indexed_with_error/
is_root: false
weight: 2050
---


## indexed_with_error property

The indicator of indexing error.

True when the document's indexing was interrupted, for example due to a cancellation. Such documents are re-indexed on the next update. Documents added from streams, structures, or extracted data cannot be re-read by the update and must be added again.

### Definition:
```python
@property
def indexed_with_error(self):
    ...
```

### See Also
* class [`DocumentInfo`](/search/python-net/groupdocs.search.results/documentinfo/)
