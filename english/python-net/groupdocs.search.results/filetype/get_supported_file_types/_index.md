---
title: get_supported_file_types method
second_title: GroupDocs.Search for Python via .NET API References
description: "Retrieves supported file types."
type: docs
url: /python-net/groupdocs.search.results/filetype/get_supported_file_types/
is_root: false
weight: 1010
---


## get_supported_file_types

Retrieves supported file types.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** list[FileType]: A collection of supported file types.

### Example

```python
    from groupdocs.search.results import FileType

    supported_file_types = sorted(
        (ft for ft in FileType.get_supported_file_types() if ft != FileType.UNKNOWN),
        key=lambda ft: ft.extension)

    for ft in supported_file_types:
        print(f"{ft.extension.ljust(8)} - {ft.description}")
    ```

### See Also
* class [`FileType`](/search/python-net/groupdocs.search.results/filetype/)
