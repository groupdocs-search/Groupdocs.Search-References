---
title: create_not method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter that has inverse logic in relation to the specified inner filter."
type: docs
url: /python-net/groupdocs.search.options/searchdocumentfilter/create_not/
is_root: false
weight: 1050
---


## create_not {#inner_filter}

Creates a filter that has inverse logic in relation to the specified inner filter.

```python
def create_not(cls, inner_filter):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| inner_filter | `ISearchDocumentFilter` | The inner search document filter. |

**Returns:** An inverted search document filter.

### Example

```python
from groupdocs.search.options import SearchDocumentFilter

filter5 = SearchDocumentFilter.create_file_extension(".txt")
not_filter = SearchDocumentFilter.create_not(filter5)
```

### See Also
* class [`SearchDocumentFilter`](/search/python-net/groupdocs.search.options/searchdocumentfilter/)
