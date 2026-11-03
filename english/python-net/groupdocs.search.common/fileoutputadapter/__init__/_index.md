---
title: __init__ constructor
second_title: GroupDocs.Search for Python via .NET API References
description: "Initializes a new instance of the FileOutputAdapter class."
type: docs
url: /python-net/groupdocs.search.common/fileoutputadapter/__init__/
is_root: false
weight: 10
---


## __init__ {#output_format-file_path}

Initializes a new instance of the [`FileOutputAdapter`](/search/python-net/groupdocs.search.common/fileoutputadapter/) class.

```python
def __init__(self, output_format, file_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| output_format | `OutputFormat` | The output format. |
| file_path | `str` | The output file path. |

### Example

```python
from groupdocs.search.common import FileOutputAdapter
from groupdocs.search.options import OutputFormat

adapter = FileOutputAdapter(OutputFormat.HTML, "./output/Highlighted.html")
```

### See Also
* class [`FileOutputAdapter`](/search/python-net/groupdocs.search.common/fileoutputadapter/)
