---
title: create_attribute method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a filter that excludes documents lacking any of the specified attributes."
type: docs
url: /python-net/groupdocs.search.options/searchdocumentfilter/create_attribute/
is_root: false
weight: 1020
---


## create_attribute {#attributes}

Creates a filter that excludes documents lacking any of the specified attributes.

```python
def create_attribute(cls, attributes):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| attributes | `list[str]` | The list of allowable attributes. |

**Returns:** SearchDocumentFilter: A filter that matches documents containing at least one of the given attributes.

### Example

```python
    import os

    from groupdocs.search import Index
    from groupdocs.search.options import SearchDocumentFilter, SearchOptions

    index = Index("./index")
    index.add("./documents")

    # Create a filter that matches documents with the "main" attribute
    document_filter = SearchDocumentFilter.create_attribute(["main"])

    # Apply the filter to a search operation
    options = SearchOptions()
    options.search_document_filter = document_filter
    result = index.search("Einstein", options)
    for found in result:
        print("Found:", os.path.basename(found.document_info.file_path))
    ```

### See Also
* class [`SearchDocumentFilter`](/search/python-net/groupdocs.search.options/searchdocumentfilter/)
