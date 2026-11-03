---
title: search_threads property
second_title: GroupDocs.Search for Python via .NET API References
description: "The number of threads used for the search."
type: docs
url: /python-net/groupdocs.search/indexsettings/search_threads/
is_root: false
weight: 2090
---


## search_threads property

The number of threads used for the search.

The default value is `NumberOfThreads.DEFAULT`, which means the search is performed using as many threads as there are processor cores (`Environment.ProcessorCount`).

The value can be changed at any time. A search uses the value that is set when the search starts.

A value changed while an index uses these settings is saved in the index immediately, or, if the index is performing an operation at that moment, when the operation finishes. A new index uses the settings with which it is created; an existing opened index uses the settings saved in it, which [`Index.index_settings`](/search/python-net/groupdocs.search/index/index_settings/) returns.

### Definition:
```python
@property
def search_threads(self):
    ...
@search_threads.setter
def search_threads(self, value):
    ...
```

### See Also
* class [`IndexSettings`](/search/python-net/groupdocs.search/indexsettings/)
