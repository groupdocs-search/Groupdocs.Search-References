---
title: MergeOptions class
second_title: GroupDocs.Search for Python via .NET API References
description: "The options for a merge operation."
type: docs
url: /python-net/groupdocs.search.options/mergeoptions/
is_root: false
weight: 260
---


## MergeOptions class

The options for a merge operation.

Learn more

- https://docs.groupdocs.com/search/python-net/merge-indexes/
- https://docs.groupdocs.com/search/python-net/optimize-index/

The MergeOptions type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.options/mergeoptions/__init__/) | Initializes a new instance of the [`MergeOptions`](/search/python-net/groupdocs.search.options/mergeoptions/) class. |

### Properties
| Property | Description |
| :- | :- |
| [cancellation](/search/python-net/groupdocs.search.options/mergeoptions/cancellation/) | The operation cancellation object, defaulting to None. |
| [is_async](/search/python-net/groupdocs.search.options/mergeoptions/is_async/) | The flag indicating whether the operation is performed asynchronously. The default value is False. |

### Example

```python
from groupdocs.search.options import MergeOptions
from groupdocs.search.common import Cancellation

options = MergeOptions()
options.cancellation = Cancellation()  # Allows the merge to be cancelled
```

### See Also
* module [`groupdocs.search.options`](/search/python-net/groupdocs.search.options/)
