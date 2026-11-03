---
title: ImageSearchOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides options for reverse image search operation."
type: docs
url: /python-net/groupdocs.search.options/imagesearchoptions/
is_root: false
weight: 210
---


## ImageSearchOptions class

Provides options for reverse image search operation.

The ImageSearchOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/imagesearchoptions/__init__/) | Initializes a new instance of the [`ImageSearchOptions`](/search/python-net/groupdocs.search.options/imagesearchoptions/) class. |

### Properties
| Property | Description |
| :- | :- |
| [hash_differences](/search/python-net/groupdocs.search.options/imagesearchoptions/hash_differences/) | The maximum number of mismatched bits in the image hash. |
| [max_result_count](/search/python-net/groupdocs.search.options/imagesearchoptions/max_result_count/) | The maximum number of found images for an image reverse search request. |
| [search_document_filter](/search/python-net/groupdocs.search.options/imagesearchoptions/search_document_filter/) | The search document filter. |

### Example

```python
from groupdocs.search.options import ImageSearchOptions
from groupdocs.search.options import SearchDocumentFilter

options = ImageSearchOptions()
options.hash_differences = 10
options.max_result_count = 100
options.search_document_filter = SearchDocumentFilter.create_file_extension(
    ".zip", ".png", ".jpg"
)
```

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
