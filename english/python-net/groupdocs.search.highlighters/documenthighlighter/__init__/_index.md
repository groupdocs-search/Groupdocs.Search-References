---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new DocumentHighlighter."
type: docs
url: /python-net/groupdocs.search.highlighters/documenthighlighter/__init__/
is_root: false
weight: 10
---


## __init__ {#output_adapter}

Initializes a new DocumentHighlighter.

```python
def __init__(self, output_adapter):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| output_adapter | `OutputAdapter` | The output adapter transferring a result of the highlighting. |

### Example

```python
from groupdocs.search.highlighters import DocumentHighlighter
from groupdocs.search.common import FileOutputAdapter
from groupdocs.search.options import OutputFormat

adapter = FileOutputAdapter(OutputFormat.HTML, "./output/Highlighted.html")
highlighter = DocumentHighlighter(adapter)
```

### See Also
* class [`DocumentHighlighter`](/search/python-net/groupdocs.search.highlighters/documenthighlighter/)
