---
title: IndexingOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides options for the indexing operation."
type: docs
url: /python-net/groupdocs.search.options/indexingoptions/
is_root: false
weight: 230
---


## IndexingOptions class

Provides options for the indexing operation.

Learn more:
- https://docs.groupdocs.com/search/python-net/indexing-options/

The IndexingOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/indexingoptions/__init__/) | Initializes a new instance of the [`IndexingOptions`](/search/python-net/groupdocs.search.options/indexingoptions/) class. |

### Properties
| Property | Description |
| :- | :- |
| [cancellation](/search/python-net/groupdocs.search.options/indexingoptions/cancellation/) | The operation cancellation object, defaulting to None. |
| [is_async](/search/python-net/groupdocs.search.options/indexingoptions/is_async/) | The flag indicating whether the operation is performed asynchronously. The default value is False. |
| [separate_process_options](/search/python-net/groupdocs.search.options/indexingoptions/separate_process_options/) | The options for extracting data in a separate process. |
| [threads](/search/python-net/groupdocs.search.options/indexingoptions/threads/) | The number of threads used for indexing (default is 1, must be between 1 and 4). |
| [auto_detect_encoding](/search/python-net/groupdocs.search.options/baseoptions/auto_detect_encoding/) | The auto_detect_encoding flag indicates whether to detect encoding automatically. The default value is False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [encoding](/search/python-net/groupdocs.search.options/baseoptions/encoding/) | The encoding used to extract text from text documents. The default is `None`, which means UTF-8 is used. If `AutoDetectEncoding` is `True`, this value serves as the default encoding. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [image_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/image_indexing_options/) | The image indexing options for reverse image search. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [metadata_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/metadata_indexing_options/) | The options for indexing metadata fields. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [ocr_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/ocr_indexing_options/) | The options for OCR processing and indexing recognized text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_backup_privilege](/search/python-net/groupdocs.search.options/baseoptions/use_backup_privilege/) | The property indicates whether the process should use the SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS to access files and directories. The default value is False. True enables privileged access using SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS; otherwise, False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_raw_text_extraction](/search/python-net/groupdocs.search.options/baseoptions/use_raw_text_extraction/) | The property indicates whether raw text extraction mode is used if possible. The default is False; raw mode can significantly increase indexing speed, while normal mode improves formatting of extracted text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |

### Example

```python
from groupdocs.search.options import IndexingOptions

def recognize(context):
    # Pass context.image_stream to your OCR engine and return the text it recognizes
    return None


# Create indexing options
options = IndexingOptions()
# Perform indexing asynchronously
options.is_async = True
# Use two threads for indexing
options.threads = 2
# Enable OCR for separate images and set the OCR connector
options.ocr_indexing_options.enabled_for_separate_images = True
options.ocr_indexing_options.ocr_connector = recognize
```

### Guides
Task guides that use `IndexingOptions`:

* [Build your first search solution](/search/python-net/guides/build-your-first-search-solution/)
* [Search index events](/search/python-net/guides/search-index-events/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
