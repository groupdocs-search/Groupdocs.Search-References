---
title: TextStorageSettings class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents the text storage settings."
type: docs
url: /python-net/groupdocs.search.options/textstoragesettings/
is_root: false
weight: 440
---


## TextStorageSettings class

Represents the text storage settings.

Learn more

- https://docs.groupdocs.com/search/python-net/storing-text-of-indexed-documents/
- https://docs.groupdocs.com/search/python-net/search-index-settings/

The TextStorageSettings type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/textstoragesettings/__init__/#compression) | Initializes a new instance of the [`TextStorageSettings`](/search/python-net/groupdocs.search.options/textstoragesettings/) class. |

### Properties
| Property | Description |
| :- | :- |
| [compression](/search/python-net/groupdocs.search.options/textstoragesettings/compression/) | The compression of text storage. The default value is `Compression.Normal`. |

### Example

```python
from groupdocs.search import IndexSettings
from groupdocs.search.options import Compression, TextStorageSettings

settings = IndexSettings()
settings.text_storage_settings = TextStorageSettings(Compression.HIGH)  # Enable storage of extracted text in the index
```

### Guides
Task guides that use `TextStorageSettings`:

* [Highlighting search results](/search/python-net/guides/highlighting-search-results/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
