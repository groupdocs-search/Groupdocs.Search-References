---
title: create_or method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a logical disjunction of the specified filters."
type: docs
url: /python-net/groupdocs.search.options/documentfilter/create_or/
is_root: false
weight: 1140
---


## create_or {#filters}

Creates a logical disjunction of the specified filters.

```python
def create_or(cls, filters):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| filters | `list[DocumentFilter]` | The document filters. |

**Returns:** DocumentFilter: A document filter that represents result of disjunction of the specified filters.

### Example

```python
    from groupdocs.search import IndexSettings
    from groupdocs.search.options import DocumentFilter

    txt_filter = DocumentFilter.create_file_extension(".txt")
    not_txt_filter = DocumentFilter.create_not(txt_filter)
    bound5_filter = DocumentFilter.create_file_length_upper_bound(5 * 1024 * 1024)
    bound10_filter = DocumentFilter.create_file_length_upper_bound(10 * 1024 * 1024)
    txt_size_filter = DocumentFilter.create_and(txt_filter, bound5_filter)
    not_txt_size_filter = DocumentFilter.create_and(not_txt_filter, bound10_filter)

    final_filter = DocumentFilter.create_or(txt_size_filter, not_txt_size_filter)

    settings = IndexSettings()
    settings.document_filter = final_filter
    print(settings.document_filter)
    ```

### See Also
* class [`DocumentFilter`](/search/python-net/groupdocs.search.options/documentfilter/)
