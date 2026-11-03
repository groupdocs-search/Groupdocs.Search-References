---
title: text_storage_settings property
second_title: GroupDocs.Search for Python via .NET API References
description: "The text storage settings."
type: docs
url: /python-net/groupdocs.search/indexsettings/text_storage_settings/
is_root: false
weight: 2110
---


## text_storage_settings property

The text storage settings. The default value is None, which means that document texts are not stored.

The setting is fixed when an index is created with these settings: a value assigned after that is ignored.

### Definition:
```python
@property
def text_storage_settings(self):
    ...
@text_storage_settings.setter
def text_storage_settings(self, value):
    ...
```

### See Also
* class [`IndexSettings`](/search/python-net/groupdocs.search/indexsettings/)
