---
title: create_or method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a logical disjunction of the specified filters."
type: docs
url: /python-net/groupdocs.search.options/searchdocumentfilter/create_or/
is_root: false
weight: 1060
---


## create_or {#filters}

Creates a logical disjunction of the specified filters.

```python
def create_or(cls, filters):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| filters | `list[ISearchDocumentFilter]` | The search document filters. |

**Returns:** A `SearchDocumentFilter` that represents the result of the disjunction of the specified filters.

### Example

```python
from groupdocs.search import RegexOptions
from groupdocs.search.options import SearchDocumentFilter

filter3 = SearchDocumentFilter.create_file_path_regular_expression(
    "Einstein", RegexOptions.IGNORE_CASE
)
filter4 = SearchDocumentFilter.create_file_extension(".doc", ".docx", ".pdf")
or_filter = SearchDocumentFilter.create_or(filter3, filter4)
```

### See Also
* class [`SearchDocumentFilter`](/search/python-net/groupdocs.search.options/searchdocumentfilter/)
