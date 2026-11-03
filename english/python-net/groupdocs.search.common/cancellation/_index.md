---
title: Cancellation class
second_title: GroupDocs.Search for Python via .NET API References
description: "Represents an object for requesting cancellation of an operation."
type: docs
url: /python-net/groupdocs.search.common/cancellation/
is_root: false
weight: 20
---


## Cancellation class

Represents an object for requesting cancellation of an operation.

Learn more

- Indexing options: https://docs.groupdocs.com/search/python-net/indexing-options/
- Search options: https://docs.groupdocs.com/search/python-net/search-options/

The Cancellation type exposes the following members:

### Constructors
| Constructor | Description |
| :- | :- |
| [__init__](/search/python-net/groupdocs.search.common/cancellation/__init__/) | Initializes a new instance of the [`Cancellation`](/search/python-net/groupdocs.search.common/cancellation/) class. |

### Methods
| Method | Description |
| :- | :- |
| [cancel](/search/python-net/groupdocs.search.common/cancellation/cancel/) | Requests cancellation of the ongoing operation. |
| [cancel_after](/search/python-net/groupdocs.search.common/cancellation/cancel_after/#milliseconds) | Makes a request for cancellation after the expiration of the specified number of milliseconds. |

### Properties
| Property | Description |
| :- | :- |
| [is_cancelled](/search/python-net/groupdocs.search.common/cancellation/is_cancelled/) | The property indicates whether cancellation has been requested. |

### Example

```python
from groupdocs.search.common import Cancellation

# Create a cancellation object that will cancel after 10 seconds (10000 ms)
cancellation = Cancellation()
cancellation.cancel_after(10000)
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
