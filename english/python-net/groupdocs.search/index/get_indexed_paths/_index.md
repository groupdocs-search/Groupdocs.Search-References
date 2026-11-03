---
title: get_indexed_paths method
second_title: GroupDocs.Search for Python via .NET API References
description: "Returns a list of indexed paths – documents or folders."
type: docs
url: /python-net/groupdocs.search/index/get_indexed_paths/
is_root: false
weight: 1110
---


## get_indexed_paths

Returns a list of indexed paths – documents or folders.

```python
def get_indexed_paths(self):
    ...
```

**Returns:** list[str]: The indexed paths.

### Example

```python
    from groupdocs.search import Index

    index = Index("./index")
    # add documents or folders to the index as needed
    indexed_paths = index.get_indexed_paths()
    print(indexed_paths)  # e.g., ['./documents', './more_docs']
    ```

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
