---
title: use_character_replacements property
second_title: GroupDocs.Search for Python via .NET API References
description: "The property indicates whether character replacements are used during indexing."
type: docs
url: /python-net/groupdocs.search/indexsettings/use_character_replacements/
is_root: false
weight: 2120
---


## use_character_replacements property

The property indicates whether character replacements are used during indexing. The default value is False.

The setting defines how the text of documents is divided into terms. Therefore, when an index uses these settings, the value can be changed only while the index contains no documents and its status is `IndexStatus.ready`.

The value is saved in the index when it is changed or, if that is not possible, before the next operation that changes the index.

A new index uses the settings object passed to its constructor until the index is disposed. If one settings object is used to create several indexes, each of them has to allow the change.

### Definition:
```python
@property
def use_character_replacements(self):
    ...
@use_character_replacements.setter
def use_character_replacements(self, value):
    ...
```

### See Also
* class [`IndexSettings`](/search/python-net/groupdocs.search/indexsettings/)
