---
title: DocumentFilter class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents the base class for document filters and provides methods to create document filter instances."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/
is_root: false
weight: 100
---


## DocumentFilter class

Represents the base class for document filters and provides methods to create document filter instances.

Learn more: Document filtering during indexing.

The DocumentFilter type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [create_and](/search/python-net/groupdocs.search.options/documentfilter/create_and/#filters) | Creates a logical conjunction of the specified filters. |
| [create_creation_time_lower_bound](/search/python-net/groupdocs.search.options/documentfilter/create_creation_time_lower_bound/#lower_bound) | Creates a filter for skipping documents with a creation date earlier than the specified lower bound. |
| [create_creation_time_range](/search/python-net/groupdocs.search.options/documentfilter/create_creation_time_range/#lower_bound-upper_bound) | Creates a filter that skips documents whose creation date is outside the specified range. |
| [create_creation_time_upper_bound](/search/python-net/groupdocs.search.options/documentfilter/create_creation_time_upper_bound/#upper_bound) | Creates a filter for skipping documents with a creation date later than the upper bound. |
| [create_file_extension](/search/python-net/groupdocs.search.options/documentfilter/create_file_extension/#extensions) | Creates a filter that skips documents without the specified extensions. |
| [create_file_length_lower_bound](/search/python-net/groupdocs.search.options/documentfilter/create_file_length_lower_bound/#lower_bound) | Creates a filter that skips documents whose length is less than the specified lower bound. |
| [create_file_length_range](/search/python-net/groupdocs.search.options/documentfilter/create_file_length_range/#lower_bound-upper_bound) | Creates a filter for skipping documents out of the specified document length range. |
| [create_file_length_upper_bound](/search/python-net/groupdocs.search.options/documentfilter/create_file_length_upper_bound/#upper_bound) | Creates a filter for skipping documents with the length greater than the upper bound. |
| [create_file_path_regular_expression](/search/python-net/groupdocs.search.options/documentfilter/create_file_path_regular_expression/#pattern) | Creates a filter that skips documents whose full path does not match a regular expression. |
| [create_file_path_regular_expression](/search/python-net/groupdocs.search.options/documentfilter/create_file_path_regular_expression/#pattern-options) | Creates a filter for skipping documents that do not match a regular expression. The regular expression is applied to the full path of a document. |
| [create_modification_time_lower_bound](/search/python-net/groupdocs.search.options/documentfilter/create_modification_time_lower_bound/#lower_bound) | Creates a filter for skipping documents with modification date earlier than the lower bound. |
| [create_modification_time_range](/search/python-net/groupdocs.search.options/documentfilter/create_modification_time_range/#lower_bound-upper_bound) | Creates a filter for skipping documents with modification date out of the specified range. |
| [create_modification_time_upper_bound](/search/python-net/groupdocs.search.options/documentfilter/create_modification_time_upper_bound/#upper_bound) | Creates a filter for skipping documents with modification dates later than the upper bound. |
| [create_not](/search/python-net/groupdocs.search.options/documentfilter/create_not/#inner_filter) | Creates a filter that inverts the logic of the specified inner filter. |
| [create_or](/search/python-net/groupdocs.search.options/documentfilter/create_or/#filters) | Creates a logical disjunction of the specified filters. |
| [to_string](/search/python-net/groupdocs.search.options/documentfilter/to_string/) | Returns string representation of a document filter. |

### Example

```python
from groupdocs.search import IndexSettings
from groupdocs.search.options import DocumentFilter
import datetime

# Include only .htm and .html files
ext_filter = DocumentFilter.create_file_extension(".htm", ".html")

# Invert the filter to exclude those extensions
filter = DocumentFilter.create_not(ext_filter)

# Apply the filter to index settings
settings = IndexSettings()
settings.document_filter = filter

print(settings.document_filter)
```

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
