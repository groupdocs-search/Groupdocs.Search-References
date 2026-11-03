---
title: get_attributes method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets all the attributes associated with the specified indexed document."
type: docs
url: /python-net/groupdocs.search.scaling/indexer/get_attributes/
is_root: false
weight: 1080
---


## get_attributes {#document_key}

Gets all the attributes associated with the specified indexed document.

```python
def get_attributes(self, document_key):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_key | `str` | The document key. |

**Returns:** list[str]: The attributes associated with the specified indexed document.

### Example

```python
from groupdocs.search.scaling import Indexer

# `indexer` should be an initialized Indexer instance
# `doc_key` is the key of the document whose attributes you want to retrieve
attributes = indexer.get_attributes(doc_key)
print("Attributes:", attributes)
```

### Aliases

These names call `get_attributes` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_attributes_file` | `get_attributes_file(document_key)` |
| `get_attributes_string` | `get_attributes_string(document_key)` |

### See Also
* class [`Indexer`](/search/python-net/groupdocs.search.scaling/indexer/)
