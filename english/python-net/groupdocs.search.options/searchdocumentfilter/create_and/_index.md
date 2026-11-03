---
title: create_and method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a logical conjunction of the specified filters."
type: docs
url: /python-net/groupdocs.search.options/searchdocumentfilter/create_and/
is_root: false
weight: 1010
---


## create_and {#filters}

Creates a logical conjunction of the specified filters.

```python
def create_and(cls, filters):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| filters | `list[ISearchDocumentFilter]` | The search document filters. |

**Returns:** SearchDocumentFilter: A search document filter that represents result of conjunction of the specified filters.

### Example

```python
from groupdocs.search import RegexOptions
from groupdocs.search.options import SearchDocumentFilter

filter1 = SearchDocumentFilter.create_file_path_regular_expression(
    "Einstein", RegexOptions.IGNORE_CASE
)
filter2 = SearchDocumentFilter.create_file_extension(".fb2", ".epub")
and_filter = SearchDocumentFilter.create_and(filter1, filter2)
```

### See Also
* class [`SearchDocumentFilter`](/search/python-net/groupdocs.search.options/searchdocumentfilter/)
