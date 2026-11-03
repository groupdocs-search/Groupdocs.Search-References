---
title: Document class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents the base class for documents added to an index from a file system, stream, or structure, and provides static methods for creating documents from different source types."
type: docs
url: /python-net/groupdocs.search.common/document/
is_root: false
weight: 50
---


## Document class

Represents the base class for documents added to an index from a file system, stream, or structure, and provides static methods for creating documents from different source types.

Learn more:
- https://docs.groupdocs.com/search/python-net/indexing-from-different-sources/

The Document type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [create_from_file](/search/python-net/groupdocs.search.common/document/create_from_file/#file_path) | Creates a document from a file. |
| [create_from_stream](/search/python-net/groupdocs.search.common/document/create_from_stream/#document_key-modification_date-extension-stream) | Creates a document from a stream. |
| [create_from_structure](/search/python-net/groupdocs.search.common/document/create_from_structure/#document_key-modification_date-fields) | Creates a document from a structure that is an array of text fields. |
| [create_lazy](/search/python-net/groupdocs.search.common/document/create_lazy/#document_source_kind-document_key-document_loader) | Creates a lazy-loaded document. |
| [to_string](/search/python-net/groupdocs.search.common/document/to_string/) | Returns a str that represents the current Document. |

### Properties
| Property | Description |
| :- | :- |
| [additional_fields](/search/python-net/groupdocs.search.common/document/additional_fields/) | The additional fields for the document. |
| [attributes](/search/python-net/groupdocs.search.common/document/attributes/) | The attributes of the document. |
| [document_key](/search/python-net/groupdocs.search.common/document/document_key/) | The document key that is used to identify the document within an index. |
| [document_source_kind](/search/python-net/groupdocs.search.common/document/document_source_kind/) | The document source kind. |
| [extension](/search/python-net/groupdocs.search.common/document/extension/) | The extension used for this document type. |
| [is_lazy](/search/python-net/groupdocs.search.common/document/is_lazy/) | The document is loaded lazily, indicating whether it is loaded as needed. |
| [modification_date](/search/python-net/groupdocs.search.common/document/modification_date/) | The last modification date of the document. |

### Guides
Task guides that use `Document`:

* [Search index events](/search/python-net/guides/search-index-events/)

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
