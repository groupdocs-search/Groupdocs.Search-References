---
title: FileOutputAdapter class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents an output adapter that collects output into a file."
type: docs
url: /python-net/groupdocs.search.common/fileoutputadapter/
is_root: false
weight: 150
---


## FileOutputAdapter class

Represents an output adapter that collects output into a file.

Learn more:

- [Output adapters](https://docs.groupdocs.com/search/python-net/output-adapters/)

The FileOutputAdapter type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.common/fileoutputadapter/__init__/#output_format-file_path) | Initializes a new instance of the [`FileOutputAdapter`](/search/python-net/groupdocs.search.common/fileoutputadapter/) class. |

### Properties
| Property | Description |
| :- | :- |
| [file_path](/search/python-net/groupdocs.search.common/fileoutputadapter/file_path/) | The output file path. |
| [output_format](/search/python-net/groupdocs.search.common/resultbuilderfactory/output_format/) | The output format. (inherited from [`ResultBuilderFactory`](/search/python-net/groupdocs.search.common/resultbuilderfactory/)) |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.common import FileOutputAdapter
from groupdocs.search.highlighters import DocumentHighlighter
from groupdocs.search.options import OutputFormat

with Index("./index") as index:
    result = index.search("Einstein")
    if result.document_count > 0:
        adapter = FileOutputAdapter(OutputFormat.HTML, "./output/Highlighted.html")
        highlighter = DocumentHighlighter(adapter)
        index.highlight(result.get_found_document(0), highlighter)
```

### Guides
Task guides that use `FileOutputAdapter`:

* [Build your first search solution](/search/python-net/guides/build-your-first-search-solution/)
* [Work with search results](/search/python-net/guides/work-with-search-results/)

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
