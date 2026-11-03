---
title: StreamOutputAdapter class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents an output adapter that collects output into a io.RawIOBase."
type: docs
url: /python-net/groupdocs.search.common/streamoutputadapter/
is_root: false
weight: 310
---


## StreamOutputAdapter class

Represents an output adapter that collects output into a `io.RawIOBase`.

Learn more

- [Output adapters](https://docs.groupdocs.com/search/python-net/output-adapters/)

The StreamOutputAdapter type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.common/streamoutputadapter/__init__/#output_format-stream) | Initializes a new instance of the [`StreamOutputAdapter`](/search/python-net/groupdocs.search.common/streamoutputadapter/) class. |

### Properties
| Property | Description |
| :- | :- |
| [stream](/search/python-net/groupdocs.search.common/streamoutputadapter/stream/) | The output stream. |
| [output_format](/search/python-net/groupdocs.search.common/resultbuilderfactory/output_format/) | The output format. (inherited from [`ResultBuilderFactory`](/search/python-net/groupdocs.search.common/resultbuilderfactory/)) |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.common import StreamOutputAdapter
from groupdocs.search.options import OutputFormat

# Create an index in the specified folder and index documents
index = Index("./MyIndex")
index.add("./documents")

# Get information on indexed documents
documents = index.get_indexed_documents()

# Write the text of the first document into a file
with open("document.html", "wb") as stream:
    adapter = StreamOutputAdapter(OutputFormat.HTML, stream)
    index.get_document_text(documents[0], adapter)
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
