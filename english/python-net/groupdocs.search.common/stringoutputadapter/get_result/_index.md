---
title: get_result method
second_title: GroupDocs.Search for Python via .NET API References
description: "Gets the resulting string."
type: docs
url: /python-net/groupdocs.search.common/stringoutputadapter/get_result/
is_root: false
weight: 1010
---


## get_result

Gets the resulting string.

```python
def get_result(self):
    ...
```

**Returns:** str: The resulting string.

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
text = adapter.get_result()
print(text[:200])
```

### See Also
* class [`StringOutputAdapter`](/search/python-net/groupdocs.search.common/stringoutputadapter/)
