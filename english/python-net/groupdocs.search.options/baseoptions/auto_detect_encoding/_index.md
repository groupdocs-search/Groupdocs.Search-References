---
title: auto_detect_encoding property
second_title: GroupDocs.Search for Python via .NET API References
description: "The auto_detect_encoding flag indicates whether to detect encoding automatically."
type: docs
url: /python-net/groupdocs.search.options/baseoptions/auto_detect_encoding/
is_root: false
weight: 2010
---


## auto_detect_encoding property

The auto_detect_encoding flag indicates whether to detect encoding automatically. The default value is False.

The auto_detect_encoding property is a flag that allows automatic detection of the following text file encodings during indexing: UTF-32 LE, UTF-32 BE, UTF-16 LE, UTF-16 BE, UTF-8, UTF-7. By default, automatic detection is disabled.

### Definition:
```python
@property
def auto_detect_encoding(self):
    ...
@auto_detect_encoding.setter
def auto_detect_encoding(self, value):
    ...
```

### See Also
* class [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)
