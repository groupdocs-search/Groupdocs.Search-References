---
title: BaseOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides base options for index operations."
type: docs
url: /python-net/groupdocs.search.options/baseoptions/
is_root: false
weight: 10
---


## BaseOptions class

Provides base options for index operations.

The BaseOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/baseoptions/__init__/) | Initializes a new instance of the [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/) class. |

### Properties
| Property | Description |
| :- | :- |
| [auto_detect_encoding](/search/python-net/groupdocs.search.options/baseoptions/auto_detect_encoding/) | The auto_detect_encoding flag indicates whether to detect encoding automatically. The default value is False. |
| [encoding](/search/python-net/groupdocs.search.options/baseoptions/encoding/) | The encoding used to extract text from text documents. The default is `None`, which means UTF-8 is used. If `AutoDetectEncoding` is `True`, this value serves as the default encoding. |
| [image_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/image_indexing_options/) | The image indexing options for reverse image search. |
| [metadata_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/metadata_indexing_options/) | The options for indexing metadata fields. |
| [ocr_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/ocr_indexing_options/) | The options for OCR processing and indexing recognized text. |
| [use_backup_privilege](/search/python-net/groupdocs.search.options/baseoptions/use_backup_privilege/) | The property indicates whether the process should use the SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS to access files and directories. The default value is False. True enables privileged access using SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS; otherwise, False. |
| [use_raw_text_extraction](/search/python-net/groupdocs.search.options/baseoptions/use_raw_text_extraction/) | The property indicates whether raw text extraction mode is used if possible. The default is False; raw mode can significantly increase indexing speed, while normal mode improves formatting of extracted text. |

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
