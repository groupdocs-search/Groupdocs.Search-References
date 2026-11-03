---
title: highlight method
second_title: GroupDocs.Search for Python via .NET API References
description: "Generates HTML formatted text with highlighted found terms."
type: docs
url: /python-net/groupdocs.search.scaling/searcher/highlight/
is_root: false
weight: 1040
---


## highlight {#document-highlighter-options}

Generates HTML formatted text with highlighted found terms.

Search results in the search network can be highlighted in the text of the found document using this method. The found document is passed as a [`NetworkFoundDocument`](/search/python-net/groupdocs.search.scaling.results/networkfounddocument/) object obtained from a search result.

```python
def highlight(self, document, highlighter, options):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document | `NetworkFoundDocument` | The found document. |
| highlighter | `Highlighter` | The search result highlighter. |
| options | `HighlightOptions` | The highlight options. |

**Returns:** None.

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

### Aliases

These names call `highlight` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `highlight_network_found_document` | `highlight_network_found_document(document, highlighter, options)` |

### See Also
* class [`Searcher`](/search/python-net/groupdocs.search.scaling/searcher/)
