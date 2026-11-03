---
title: TextOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides options for retrieving document text from an index."
type: docs
url: /python-net/groupdocs.search.options/textoptions/
is_root: false
weight: 430
---


## TextOptions class

Provides options for retrieving document text from an index.

- Getting indexed documents: https://docs.groupdocs.com/search/python-net/getting-indexed-documents/
- Highlighting search results: https://docs.groupdocs.com/search/python-net/highlighting-search-results/

The TextOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/textoptions/__init__/) | Initializes a new instance of the TextOptions class. |

### Properties
| Property | Description |
| :- | :- |
| [additional_fields](/search/python-net/groupdocs.search.options/textoptions/additional_fields/) | The additional document fields that was used for indexing. The default value is `None`. |
| [cancellation](/search/python-net/groupdocs.search.options/textoptions/cancellation/) | The cancellation object. The default value is None. |
| [custom_extractor](/search/python-net/groupdocs.search.options/textoptions/custom_extractor/) | The custom text extractor that was used for indexing. The default value is None. This value is used only if document text was not saved into the index. |
| [generate_head](/search/python-net/groupdocs.search.options/textoptions/generate_head/) | The generate_head property indicates whether the Head tag is generated in the output HTML. |
| [auto_detect_encoding](/search/python-net/groupdocs.search.options/baseoptions/auto_detect_encoding/) | The auto_detect_encoding flag indicates whether to detect encoding automatically. The default value is False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [encoding](/search/python-net/groupdocs.search.options/baseoptions/encoding/) | The encoding used to extract text from text documents. The default is `None`, which means UTF-8 is used. If `AutoDetectEncoding` is `True`, this value serves as the default encoding. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [image_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/image_indexing_options/) | The image indexing options for reverse image search. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [metadata_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/metadata_indexing_options/) | The options for indexing metadata fields. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [ocr_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/ocr_indexing_options/) | The options for OCR processing and indexing recognized text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_backup_privilege](/search/python-net/groupdocs.search.options/baseoptions/use_backup_privilege/) | The property indicates whether the process should use the SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS to access files and directories. The default value is False. True enables privileged access using SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS; otherwise, False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_raw_text_extraction](/search/python-net/groupdocs.search.options/baseoptions/use_raw_text_extraction/) | The property indicates whether raw text extraction mode is used if possible. The default is False; raw mode can significantly increase indexing speed, while normal mode improves formatting of extracted text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
