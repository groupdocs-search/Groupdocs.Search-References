---
title: StringOutputAdapter class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents an output adapter that collects output as a str."
type: docs
url: /python-net/groupdocs.search.common/stringoutputadapter/
is_root: false
weight: 320
---


## StringOutputAdapter class

Represents an output adapter that collects output as a str.

Learn more

- Output adapters: https://docs.groupdocs.com/search/python-net/output-adapters/

The StringOutputAdapter type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.common/stringoutputadapter/__init__/#output_format) | Initializes a new instance of the StringOutputAdapter class. |

### Methods
| Method | Description |
| :- | :- |
| [get_result](/search/python-net/groupdocs.search.common/stringoutputadapter/get_result/) | Gets the resulting string. |

### Properties
| Property | Description |
| :- | :- |
| [output_format](/search/python-net/groupdocs.search.common/resultbuilderfactory/output_format/) | The output format. (inherited from [`ResultBuilderFactory`](/search/python-net/groupdocs.search.common/resultbuilderfactory/)) |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.common import StringOutputAdapter
from groupdocs.search.options import OutputFormat

index = Index("./index")
index.add("./documents")
documents = index.get_indexed_documents()
adapter = StringOutputAdapter(OutputFormat.PLAIN_TEXT)
index.get_document_text(documents[0], adapter)
print(adapter.get_result()[:200])
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
