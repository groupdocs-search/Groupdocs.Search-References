---
title: IndexSettings class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents the index settings that allow customizing the indexing operations."
type: docs
url: /python-net/groupdocs.search/indexsettings/
is_root: false
weight: 60
---


## IndexSettings class

Represents the index settings that allow customizing the indexing operations.

Learn more:
- https://docs.groupdocs.com/search/python-net/search-index-settings/

The IndexSettings type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search/indexsettings/__init__/) | Initializes a new instance of the [`IndexSettings`](/search/python-net/groupdocs.search/indexsettings/) class. |

### Properties
| Property | Description |
| :- | :- |
| [custom_extractors](/search/python-net/groupdocs.search/indexsettings/custom_extractors/) | The custom extractor collection. |
| [document_filter](/search/python-net/groupdocs.search/indexsettings/document_filter/) | The document filter applied during indexing; when `None`, all added documents are indexed. |
| [in_memory_index](/search/python-net/groupdocs.search/indexsettings/in_memory_index/) | The property returns a value indicating whether the index is stored in memory or on disk. |
| [index_type](/search/python-net/groupdocs.search/indexsettings/index_type/) | The index type. The default value is `IndexType.normal_index`. |
| [logger](/search/python-net/groupdocs.search/indexsettings/logger/) | The logger used for logging events and errors in the index; it is not saved and must be created and assigned each time the index is created or loaded. |
| [max_indexing_report_count](/search/python-net/groupdocs.search/indexsettings/max_indexing_report_count/) | The maximum number of indexing reports. The default value is 5. |
| [max_search_report_count](/search/python-net/groupdocs.search/indexsettings/max_search_report_count/) | The maximum number of search reports, defaulting to 10. |
| [replace_unpaired_surrogates](/search/python-net/groupdocs.search/indexsettings/replace_unpaired_surrogates/) | The flag for replacing unpaired surrogates. The default value is True. |
| [search_threads](/search/python-net/groupdocs.search/indexsettings/search_threads/) | The number of threads used for the search. |
| [skip_blended_only_terms](/search/python-net/groupdocs.search/indexsettings/skip_blended_only_terms/) | The flag indicating whether to skip terms consisting solely of blended characters. The default value is True. |
| [text_storage_settings](/search/python-net/groupdocs.search/indexsettings/text_storage_settings/) | The text storage settings. The default value is None, which means that document texts are not stored. |
| [use_character_replacements](/search/python-net/groupdocs.search/indexsettings/use_character_replacements/) | The property indicates whether character replacements are used during indexing. The default value is False. |
| [use_stop_words](/search/python-net/groupdocs.search/indexsettings/use_stop_words/) | The flag indicating whether to use stop words during indexing. The default value is True. |

### Example

```python
from groupdocs.search import Index, IndexSettings
from groupdocs.search.options import IndexType

settings = IndexSettings()
settings.index_type = IndexType.COMPACT_INDEX  # Set the index type

index = Index("./MyIndex", settings)  # Create an index with the specified settings
```

### Guides
Task guides that use `IndexSettings`:

* [Highlighting search results](/search/python-net/guides/highlighting-search-results/)
* [Custom text extractors](/search/python-net/guides/custom-text-extractors/)

### See Also
* module [`groupdocs.search`](/search/python-net/groupdocs.search/)
