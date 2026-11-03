---
title: ExtractionOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides options for extracting data from documents."
type: docs
url: /python-net/groupdocs.search.options/extractionoptions/
is_root: false
weight: 120
---


## ExtractionOptions class

Provides options for extracting data from documents.

The ExtractionOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/extractionoptions/__init__/) | Initializes a new instance of the [`ExtractionOptions`](/search/python-net/groupdocs.search.options/extractionoptions/) class. |

### Properties
| Property | Description |
| :- | :- |
| [custom_extractor](/search/python-net/groupdocs.search.options/extractionoptions/custom_extractor/) | The custom text extractor. The default value is None. |
| [auto_detect_encoding](/search/python-net/groupdocs.search.options/baseoptions/auto_detect_encoding/) | The auto_detect_encoding flag indicates whether to detect encoding automatically. The default value is False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [encoding](/search/python-net/groupdocs.search.options/baseoptions/encoding/) | The encoding used to extract text from text documents. The default is `None`, which means UTF-8 is used. If `AutoDetectEncoding` is `True`, this value serves as the default encoding. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [image_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/image_indexing_options/) | The image indexing options for reverse image search. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [metadata_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/metadata_indexing_options/) | The options for indexing metadata fields. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [ocr_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/ocr_indexing_options/) | The options for OCR processing and indexing recognized text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_backup_privilege](/search/python-net/groupdocs.search.options/baseoptions/use_backup_privilege/) | The property indicates whether the process should use the SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS to access files and directories. The default value is False. True enables privileged access using SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS; otherwise, False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_raw_text_extraction](/search/python-net/groupdocs.search.options/baseoptions/use_raw_text_extraction/) | The property indicates whether raw text extraction mode is used if possible. The default is False; raw mode can significantly increase indexing speed, while normal mode improves formatting of extracted text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |

### Example

```python
from groupdocs.search import Extractor
from groupdocs.search.common import Document
from groupdocs.search.options import ExtractionOptions

extractor = Extractor()
extractor.error_occurred += lambda sender, args: print(args.message)

document = Document.create_from_file("./documents/lecture.txt")

extraction_options = ExtractionOptions()
extraction_options.use_raw_text_extraction = False

extracted_data = extractor.extract(document, extraction_options)
```

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
