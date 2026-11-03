---
title: HighlightOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "Provides options for highlighting found terms."
type: docs
url: /python-net/groupdocs.search.options/highlightoptions/
is_root: false
weight: 160
---


## HighlightOptions class

Provides options for highlighting found terms.

Learn more

- https://docs.groupdocs.com/search/python-net/highlighting-search-results/

The HighlightOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/highlightoptions/__init__/) | Initializes a new instance of the [`HighlightOptions`](/search/python-net/groupdocs.search.options/highlightoptions/) class. |

### Properties
| Property | Description |
| :- | :- |
| [highlight_color](/search/python-net/groupdocs.search.options/highlightoptions/highlight_color/) | The color used to highlight occurrences (default is #FFD800). |
| [term_highlight_end_tag](/search/python-net/groupdocs.search.options/highlightoptions/term_highlight_end_tag/) | The end tag of the highlighting of the found word. |
| [term_highlight_start_tag](/search/python-net/groupdocs.search.options/highlightoptions/term_highlight_start_tag/) | The start tag used to highlight a found word in plain‑text results. |
| [terms_after](/search/python-net/groupdocs.search.options/highlightoptions/terms_after/) | The maximum number of words in a text fragment after a highlighted word. |
| [terms_before](/search/python-net/groupdocs.search.options/highlightoptions/terms_before/) | The maximum number of words in a text fragment before highlighted word. |
| [terms_total](/search/python-net/groupdocs.search.options/highlightoptions/terms_total/) | The maximum number of words in a text fragment. The value must be in the range from 0 to 10000. The default value is 21. |
| [use_inline_styles](/search/python-net/groupdocs.search.options/highlightoptions/use_inline_styles/) | The value indicating whether inline styles are used to highlight occurrences. The default value is True. |
| [additional_fields](/search/python-net/groupdocs.search.options/textoptions/additional_fields/) | The additional document fields that was used for indexing. The default value is `None`. (inherited from [`TextOptions`](/search/python-net/groupdocs.search.options/textoptions/)) |
| [auto_detect_encoding](/search/python-net/groupdocs.search.options/baseoptions/auto_detect_encoding/) | The auto_detect_encoding flag indicates whether to detect encoding automatically. The default value is False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [cancellation](/search/python-net/groupdocs.search.options/textoptions/cancellation/) | The cancellation object. The default value is None. (inherited from [`TextOptions`](/search/python-net/groupdocs.search.options/textoptions/)) |
| [custom_extractor](/search/python-net/groupdocs.search.options/textoptions/custom_extractor/) | The custom text extractor that was used for indexing. The default value is None. This value is used only if document text was not saved into the index. (inherited from [`TextOptions`](/search/python-net/groupdocs.search.options/textoptions/)) |
| [encoding](/search/python-net/groupdocs.search.options/baseoptions/encoding/) | The encoding used to extract text from text documents. The default is `None`, which means UTF-8 is used. If `AutoDetectEncoding` is `True`, this value serves as the default encoding. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [generate_head](/search/python-net/groupdocs.search.options/textoptions/generate_head/) | The generate_head property indicates whether the Head tag is generated in the output HTML. (inherited from [`TextOptions`](/search/python-net/groupdocs.search.options/textoptions/)) |
| [image_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/image_indexing_options/) | The image indexing options for reverse image search. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [metadata_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/metadata_indexing_options/) | The options for indexing metadata fields. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [ocr_indexing_options](/search/python-net/groupdocs.search.options/baseoptions/ocr_indexing_options/) | The options for OCR processing and indexing recognized text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_backup_privilege](/search/python-net/groupdocs.search.options/baseoptions/use_backup_privilege/) | The property indicates whether the process should use the SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS to access files and directories. The default value is False. True enables privileged access using SeBackupPrivilege and FILE_FLAG_BACKUP_SEMANTICS; otherwise, False. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |
| [use_raw_text_extraction](/search/python-net/groupdocs.search.options/baseoptions/use_raw_text_extraction/) | The property indicates whether raw text extraction mode is used if possible. The default is False; raw mode can significantly increase indexing speed, while normal mode improves formatting of extracted text. (inherited from [`BaseOptions`](/search/python-net/groupdocs.search.options/baseoptions/)) |

### Example

```python
from groupdocs.search.options import Color, HighlightOptions

options = HighlightOptions()
options.terms_before = 5
options.terms_after = 5
options.terms_total = 15
options.highlight_color = Color(0, 0, 127)
options.use_inline_styles = True
```

### Guides
Task guides that use `HighlightOptions`:

* [Highlighting search results](/search/python-net/guides/highlighting-search-results/)

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
