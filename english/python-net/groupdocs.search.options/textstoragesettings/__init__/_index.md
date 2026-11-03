---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new instance of the TextStorageSettings class."
type: docs
url: /python-net/groupdocs.search.options/textstoragesettings/__init__/
is_root: false
weight: 10
---


## __init__ {#compression}

Initializes a new instance of the [`TextStorageSettings`](/search/python-net/groupdocs.search.options/textstoragesettings/) class.

```python
def __init__(self, compression):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| compression | `Compression` | The compression of text storage. |

### Example

```python
from groupdocs.search import IndexSettings
from groupdocs.search.options import TextStorageSettings, Compression

settings = IndexSettings()
settings.text_storage_settings = TextStorageSettings(Compression.HIGH)  # Enable storage of extracted text in the index
```

### See Also
* class [`TextStorageSettings`](/search/python-net/groupdocs.search.options/textstoragesettings/)
