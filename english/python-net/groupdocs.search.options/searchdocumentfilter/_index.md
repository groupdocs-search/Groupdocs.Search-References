---
title: SearchDocumentFilter class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides methods for creating search document filters."
type: docs
url: /python-net/groupdocs.search.options/searchdocumentfilter/
is_root: false
weight: 340
---


## SearchDocumentFilter class

Provides methods for creating search document filters.

Learn more:
- https://docs.groupdocs.com/search/python-net/document-filtering-in-search-result/
- https://docs.groupdocs.com/search/python-net/search-options/

The SearchDocumentFilter type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [create_and](/search/python-net/groupdocs.search.options/searchdocumentfilter/create_and/#filters) | Creates a logical conjunction of the specified filters. |
| [create_attribute](/search/python-net/groupdocs.search.options/searchdocumentfilter/create_attribute/#attributes) | Creates a filter that excludes documents lacking any of the specified attributes. |
| [create_file_extension](/search/python-net/groupdocs.search.options/searchdocumentfilter/create_file_extension/#extensions) | Creates a filter for skipping documents that are not in the specified list of possible extensions. |
| [create_file_path_regular_expression](/search/python-net/groupdocs.search.options/searchdocumentfilter/create_file_path_regular_expression/#pattern) | Creates a filter that skips documents whose full path does not match the given regular expression. |
| [create_file_path_regular_expression](/search/python-net/groupdocs.search.options/searchdocumentfilter/create_file_path_regular_expression/#pattern-options) | Creates a filter that skips documents not matching a regular expression. |
| [create_not](/search/python-net/groupdocs.search.options/searchdocumentfilter/create_not/#inner_filter) | Creates a filter that has inverse logic in relation to the specified inner filter. |
| [create_or](/search/python-net/groupdocs.search.options/searchdocumentfilter/create_or/#filters) | Creates a logical disjunction of the specified filters. |

### Example

```python
from groupdocs.search import RegexOptions
from groupdocs.search.options import SearchDocumentFilter

# Filter documents that have the attribute "main"
attribute_filter = SearchDocumentFilter.create_attribute("main")

# Filter files whose path contains "Einstein" (case‑insensitive)
path_filter = SearchDocumentFilter.create_file_path_regular_expression(
    "Einstein", RegexOptions.IGNORE_CASE
)

# Exclude TXT files from results
txt_filter = SearchDocumentFilter.create_file_extension(".txt")
not_txt_filter = SearchDocumentFilter.create_not(txt_filter)
```

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
