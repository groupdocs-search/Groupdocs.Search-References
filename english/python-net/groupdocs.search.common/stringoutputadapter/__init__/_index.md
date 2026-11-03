---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new instance of the StringOutputAdapter class."
type: docs
url: /python-net/groupdocs.search.common/stringoutputadapter/__init__/
is_root: false
weight: 10
---


## __init__ {#output_format}

Initializes a new instance of the StringOutputAdapter class.

```python
def __init__(self, output_format):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| output_format | `OutputFormat` | The output format. |

### Example

```python
from groupdocs.search.common import StringOutputAdapter
from groupdocs.search.options import OutputFormat

adapter = StringOutputAdapter(OutputFormat.PLAIN_TEXT)
```

### See Also
* class [`StringOutputAdapter`](/search/python-net/groupdocs.search.common/stringoutputadapter/)
