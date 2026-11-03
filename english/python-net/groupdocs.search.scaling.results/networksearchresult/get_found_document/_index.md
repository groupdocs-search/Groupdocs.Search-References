---
title: get_found_document method
second_title: GroupDocs.Search for Python via .NET API References
description: "Retrieves the found document by its index."
type: docs
url: /python-net/groupdocs.search.scaling.results/networksearchresult/get_found_document/
is_root: false
weight: 1020
---


## get_found_document {#index}

Retrieves the found document by its index.

In evaluation mode only the first 10 found documents are accessible. The `document_count` property reports the total number of matches, but calling `get_found_document` with an index of 10 or greater raises `LicenseRestrictionException` with the message "Only first 10 results can be returned".

```python
def get_found_document(self, index):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| index | `int` | The index of a found document. |

**Returns:** GroupDocs.Search.Scaling.Results.FoundDocument: The found document.

| Raises | Description |
| :- | :- |
| `LicenseRestrictionException` | If `index` is 10 or greater in evaluation mode. |

### Example

```python
from groupdocs.search import Index

index = Index("./index")
index.add("./documents")

result = index.search("contract")
count = min(result.document_count, 10)  # Only the first 10 found documents are available in the evaluation mode
for i in range(count):
    document = result.get_found_document(i)
    print(document.document_info.file_path)
```

### Aliases

These names call `get_found_document` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_found_document_int32` | `get_found_document_int32(index)` |

### See Also
* class [`NetworkSearchResult`](/search/python-net/groupdocs.search.scaling.results/networksearchresult/)
