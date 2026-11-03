---
title: DocumentHighlighter class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents a search result highlighter that highlights search results in an entire document text."
type: docs
url: /python-net/groupdocs.search.highlighters/documenthighlighter/
is_root: false
weight: 10
---


## DocumentHighlighter class

Represents a search result highlighter that highlights search results in an entire document text.

Learn more

- https://docs.groupdocs.com/search/python-net/highlighting-search-results/

The DocumentHighlighter type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.highlighters/documenthighlighter/__init__/#output_adapter) | Initializes a new DocumentHighlighter. |

### Properties
| Property | Description |
| :- | :- |
| [output_adapter](/search/python-net/groupdocs.search.highlighters/documenthighlighter/output_adapter/) | The output adapter passed in the constructor. |
| [output_format](/search/python-net/groupdocs.search.common/resultbuilderfactory/output_format/) | The output format. (inherited from [`ResultBuilderFactory`](/search/python-net/groupdocs.search.common/resultbuilderfactory/)) |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.common import FileOutputAdapter
from groupdocs.search.highlighters import DocumentHighlighter
from groupdocs.search.options import OutputFormat

index = Index("./index")
index.add("./documents")
result = index.search("Einstein")

if result.document_count > 0:
    adapter = FileOutputAdapter(OutputFormat.HTML, "./output/Highlighted.html")
    highlighter = DocumentHighlighter(adapter)
    index.highlight(result.get_found_document(0), highlighter)
```

### Guides
Task guides that use `DocumentHighlighter`:

* [Build your first search solution](/search/python-net/guides/build-your-first-search-solution/)
* [Work with search results](/search/python-net/guides/work-with-search-results/)
* [Highlighting search results](/search/python-net/guides/highlighting-search-results/)

### See Also
* module [`groupdocs.search.highlighters`](/search/python-net/groupdocs.search.highlighters/)
