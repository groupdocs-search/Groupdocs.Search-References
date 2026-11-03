---
title: DocumentInfo class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a descriptor for an indexed document."
type: docs
url: /python-net/groupdocs.search.results/documentinfo/
is_root: false
weight: 20
---


## DocumentInfo class

Represents a descriptor for an indexed document.

Learn more

- Search results: https://docs.groupdocs.com/search/python-net/search-results/
- Getting indexed documents: https://docs.groupdocs.com/search/python-net/getting-indexed-documents/

The DocumentInfo type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [deserialize](/search/python-net/groupdocs.search.results/documentinfo/deserialize/#array) | Deserializes a DocumentInfo instance from a byte array. |
| [serialize](/search/python-net/groupdocs.search.results/documentinfo/serialize/) | Serializes the current instance to a byte array. |
| [to_string](/search/python-net/groupdocs.search.results/documentinfo/to_string/) | Returns a string that represents the current DocumentInfo. |

### Properties
| Property | Description |
| :- | :- |
| [document_source_kind](/search/python-net/groupdocs.search.results/documentinfo/document_source_kind/) | The document source kind. |
| [file_path](/search/python-net/groupdocs.search.results/documentinfo/file_path/) | The file path for a document indexed from a file, or the document key for a document indexed from a stream or structure. |
| [file_type](/search/python-net/groupdocs.search.results/documentinfo/file_type/) | The file type. |
| [format_family](/search/python-net/groupdocs.search.results/documentinfo/format_family/) | The document format family. |
| [indexed_with_error](/search/python-net/groupdocs.search.results/documentinfo/indexed_with_error/) | The indicator of indexing error. |
| [inner_path](/search/python-net/groupdocs.search.results/documentinfo/inner_path/) | The inner path for the container document item. |
| [inner_path_parts](/search/python-net/groupdocs.search.results/documentinfo/inner_path_parts/) | The inner path parts for the container document item. |
| [modification_time](/search/python-net/groupdocs.search.results/documentinfo/modification_time/) | The modification time of the document. |

### Example

```python
from groupdocs.search import Index

index = Index("./index")
for doc in index.get_indexed_documents():
    print(doc.file_path)
```

### See Also
* module [`groupdocs.search.results`](/search/python-net/groupdocs.search.results/)
