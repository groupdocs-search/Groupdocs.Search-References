---
title: create_not method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter that inverts the logic of the specified inner filter."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_not/
is_root: false
weight: 1130
---


## create_not {#inner_filter}

Creates a filter that inverts the logic of the specified inner filter.

```python
def create_not(cls, inner_filter):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| inner_filter | `DocumentFilter` | The inner document filter. |

**Returns:** DocumentFilter: An inverted document filter.

### Example

```python
    from groupdocs.search import IndexSettings
    from groupdocs.search.options import DocumentFilter

    settings = IndexSettings()
    document_filter = DocumentFilter.create_file_extension(".htm", ".html")
    inverted_filter = DocumentFilter.create_not(document_filter)  # Invert file extension filter
    settings.document_filter = inverted_filter

    print(settings.document_filter)
    ```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
