---
title: get_document_text method
second_title: GroupDocs.Search for Python via .NET API References
description: "Generates the text of an indexed document and passes it through an output adapter."
type: docs
url: /python-net/groupdocs.search.scaling/searcher/get_document_text/
is_root: false
weight: 1010
---


## get_document_text {#document_info-adapter}

Generates the text of an indexed document and passes it through an output adapter.

```python
def get_document_text(self, document_info, adapter):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| document_info | `NetworkDocumentInfo` | The indexed document info. |
| adapter | `OutputAdapter` | The output adapter. |

### Example

```python
from groupdocs.search import Index
from groupdocs.search.common import StringOutputAdapter
from groupdocs.search.options import OutputFormat

index = Index("./index")
index.add("./documents")
doc = index.get_indexed_documents()[0]

adapter = StringOutputAdapter(OutputFormat.PLAIN_TEXT)
index.get_document_text(doc, adapter)
print(adapter.get_result()[:200])
```

### Aliases

These names call `get_document_text` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `get_document_text_network_document_info` | `get_document_text_network_document_info(document_info, adapter)` |

### See Also
* class [`Searcher`](/search/python-net/groupdocs.search.scaling/searcher/)
