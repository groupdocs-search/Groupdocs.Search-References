---
title: FoundDocument class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a found document."
type: docs
url: /python-net/groupdocs.search.results/founddocument/
is_root: false
weight: 50
---


## FoundDocument class

Represents a found document.

Learn more:
- https://docs.groupdocs.com/search/python-net/search-results/

The FoundDocument type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [deserialize](/search/python-net/groupdocs.search.results/founddocument/deserialize/#array) | Deserializes a FoundDocument instance from a byte array. |
| [serialize](/search/python-net/groupdocs.search.results/founddocument/serialize/) | Serializes the current instance to a byte array. |
| [to_string](/search/python-net/groupdocs.search.results/founddocument/to_string/) | Returns a string representation of the found document. |

### Properties
| Property | Description |
| :- | :- |
| [attributes](/search/python-net/groupdocs.search.results/founddocument/attributes/) | The attributes associated with the found document. The corresponding option must be enabled in the search options to retrieve attributes. |
| [document_info](/search/python-net/groupdocs.search.results/founddocument/document_info/) | The document info. |
| [found_fields](/search/python-net/groupdocs.search.results/founddocument/found_fields/) | The document fields found. |
| [occurrence_count](/search/python-net/groupdocs.search.results/founddocument/occurrence_count/) | The number of occurrences found. |
| [relevance](/search/python-net/groupdocs.search.results/founddocument/relevance/) | The relevance of search result. |
| [term_sequences](/search/python-net/groupdocs.search.results/founddocument/term_sequences/) | The term sequences found. |
| [terms](/search/python-net/groupdocs.search.results/founddocument/terms/) | The terms found; the value is evaluated each time the property is accessed. |

### Example

```python
from groupdocs.search import Index

index = Index("./index")
index.add("./documents")
result = index.search("contract")
for found in result:  # FoundDocument
    print(found.document_info.file_path, found.occurrence_count, found.relevance)
    print("fields:", [f.field_name for f in found.found_fields])
```

### See Also
* module [`groupdocs.search.results`](/search/python-net/groupdocs.search.results/)
