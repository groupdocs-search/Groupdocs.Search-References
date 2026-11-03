---
title: cancel_after method
second_title: GroupDocs.Search for Python via .NET API References
description: "Makes a request for cancellation after the expiration of the specified number of milliseconds."
type: docs
url: /python-net/groupdocs.search.common/cancellation/cancel_after/
is_root: false
weight: 1020
---


## cancel_after {#milliseconds}

Makes a request for cancellation after the expiration of the specified number of milliseconds.

```python
def cancel_after(self, milliseconds):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| milliseconds | `int` | The number of milliseconds after which an operation will be cancelled. |

### Example

```python
from groupdocs.search.common import Cancellation

cancellation = Cancellation()
cancellation.cancel_after(10_000)  # Cancel after 10 seconds
```

### Aliases

These names call `cancel_after` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `cancel_after_int32` | `cancel_after_int32(milliseconds)` |

### See Also
* class [`Cancellation`](/search/python-net/groupdocs.search.common/cancellation/)
