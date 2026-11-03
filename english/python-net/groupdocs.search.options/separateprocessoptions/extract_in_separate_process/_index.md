---
title: extract_in_separate_process property
second_title: GroupDocs.Search for Python via .NET API References
description: "The property indicates whether a separate process is used to extract data from documents."
type: docs
url: /python-net/groupdocs.search.options/separateprocessoptions/extract_in_separate_process/
is_root: false
weight: 2020
---


## extract_in_separate_process property

The property indicates whether a separate process is used to extract data from documents.

The default value is `False`.

When enabled, data extraction is performed in a separate process using only one thread; the configured number of threads is ignored.

### Definition:
```python
@property
def extract_in_separate_process(self):
    ...
@extract_in_separate_process.setter
def extract_in_separate_process(self, value):
    ...
```

### See Also
* class [`SeparateProcessOptions`](/search/python-net/groupdocs.search.options/separateprocessoptions/)
