---
title: use_stop_words property
second_title: GroupDocs.Search for Python via .NET API References
description: "The flag indicating whether to use stop words during indexing."
type: docs
url: /python-net/groupdocs.search/indexsettings/use_stop_words/
is_root: false
weight: 2130
---


## use_stop_words property

The flag indicating whether to use stop words during indexing. The default value is True.

The setting defines how the text of documents is divided into terms. Therefore, when an index uses these settings, the value can be changed only while the index contains no documents and its status is `IndexStatus.ready`.

The value is saved in the index when it is changed or, if that is not possible, before the next operation that changes the index.

A new index uses the settings object passed to its constructor until the index is disposed. If one settings object is used to create several indexes, each of them has to allow the change.

### Definition:
```python
@property
def use_stop_words(self):
    ...
@use_stop_words.setter
def use_stop_words(self, value):
    ...
```

### See Also
* class [`IndexSettings`](/search/python-net/groupdocs.search/indexsettings/)
