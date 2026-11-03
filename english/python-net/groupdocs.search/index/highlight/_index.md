---
title: highlight method
second_title: GroupDocs.Search for Python via .NET API References
description: "Generates HTML formatted text with highlighted found terms."
type: docs
url: /python-net/groupdocs.search/index/highlight/
is_root: false
weight: 1140
---


## highlight {#document-highlighter}

Generates HTML formatted text with highlighted found terms.

```python
def highlight(self, document, highlighter):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `FoundDocument` | The found document. |
| highlighter | `Highlighter` | The search result highlighter. |

### Example

```python
import os
from groupdocs.search import Index
from groupdocs.search.common import FileOutputAdapter
from groupdocs.search.highlighters import DocumentHighlighter
from groupdocs.search.options import OutputFormat

os.makedirs("./output", exist_ok=True)

with Index("./index") as index:
    index.add("./documents")
    result = index.search("Einstein")
    if result.document_count > 0:
        adapter = FileOutputAdapter(OutputFormat.HTML, "./output/Highlighted.html")
        highlighter = DocumentHighlighter(adapter)
        index.highlight(result.get_found_document(0), highlighter)
        print("Written: ./output/Highlighted.html")
```

## highlight {#document-highlighter-options}

Generates HTML formatted text with highlighted found terms.

```python
def highlight(self, document, highlighter, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `FoundDocument` | The found document. |
| highlighter | `Highlighter` | The search result highlighter. |
| options | `HighlightOptions` | The highlight options. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.common import FileOutputAdapter
from groupdocs.search.highlighters import DocumentHighlighter
from groupdocs.search.options import OutputFormat, HighlightOptions

with Index("./index") as index:
    result = index.search("Einstein")
    if result.document_count > 0:
        adapter = FileOutputAdapter(OutputFormat.HTML, "./output/Highlighted.html")
        highlighter = DocumentHighlighter(adapter)
        options = HighlightOptions()
        options.terms_before = 5
        options.terms_after = 5
        options.terms_total = 15
        index.highlight(result.get_found_document(0), highlighter, options)
```

### Aliases

These names call `highlight` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `highlight_found_document` | `highlight_found_document(document, highlighter, options)`<br>`highlight_found_document(document, highlighter)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
