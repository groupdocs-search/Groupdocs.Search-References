---
title: UpdateOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides options for update operation."
type: docs
url: /python-net/groupdocs.search.options/updateoptions/
is_root: false
weight: 450
---


## UpdateOptions class

Provides options for update operation.

- [Update index](https://docs.groupdocs.com/search/python-net/update-index/)
- [Delete indexed paths](https://docs.groupdocs.com/search/python-net/delete-indexed-paths/)

The UpdateOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/updateoptions/__init__/) | Initializes a new instance of the UpdateOptions class. |

### Properties
| Property | Description |
| :- | :- |
| [cancellation](/search/python-net/groupdocs.search.options/updateoptions/cancellation/) | The operation cancellation object. The default value is None. |
| [is_async](/search/python-net/groupdocs.search.options/updateoptions/is_async/) | The flag indicating whether the operation should be performed asynchronously. The default value is False. |
| [separate_process_options](/search/python-net/groupdocs.search.options/updateoptions/separate_process_options/) | The options for extracting data in a separate process. |
| [threads](/search/python-net/groupdocs.search.options/updateoptions/threads/) | The number of threads used for indexing. |
| [auto_detect_encoding](/search/python-net/groupdocs.search.options/baseoptions/auto_detect_encoding/) | The auto_detect_encoding flag indicates whether to detect encoding automatically. The default value is False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [encoding](/search/python-net/groupdocs.search.options/baseoptions/encoding/) | The encoding used to extract text from text documents. The default is `None`, which means UTF-8 is used. If `AutoDetectEncoding` is `True`, this value serves as the default encoding. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [image_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/image_indexing_options/) | The image indexing options for reverse image search. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [metadata_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/metadata_indexing_options/) | The options for indexing metadata fields. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [ocr_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/ocr_indexing_options/) | The options for OCR processing and indexing recognized text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_backup_privilege](/search/python-net/groupdocs.search.options/baseoptions/use_backup_privilege/) | The property indicates whether the process should use the SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS to access files and directories. The default value is False. True enables privileged access using SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS; otherwise, False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_raw_text_extraction](/search/python-net/groupdocs.search.options/baseoptions/use_raw_text_extraction/) | The property indicates whether raw text extraction mode is used if possible. The default is False; raw mode can significantly increase indexing speed, while normal mode improves formatting of extracted text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.options import UpdateOptions

# Delete indexed paths from the index
result = index.delete([documents_folder1], UpdateOptions())
print(f"Deleted paths: {result.success_count}")
```

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
