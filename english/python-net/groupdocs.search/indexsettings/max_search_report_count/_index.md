---
title: max_search_report_count property
second_title: GroupDocs.Search for Python via .NET API References
description: "The maximum number of search reports, defaulting to 10."
type: docs
url: /python-net/groupdocs.search/indexsettings/max_search_report_count/
is_root: false
weight: 2070
---


## max_search_report_count property

The maximum number of search reports, defaulting to 10.

The value can be changed at any time. A value changed after an index was created with these settings is saved in the index by the next operation that changes the index.

### Definition:
```python
@property
def max_search_report_count(self):
    ...
@max_search_report_count.setter
def max_search_report_count(self, value):
    ...
```

### See Also
* class [`IndexSettings`](/search/python-net/groupdocs.search/indexsettings/)
