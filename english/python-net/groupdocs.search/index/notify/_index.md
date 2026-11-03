---
title: notify method
second_title: GroupDocs.Search for Python via .NET API References
description: "Passes the specified notification object to the index to perform the notification."
type: docs
url: /python-net/groupdocs.search/index/notify/
is_root: false
weight: 1170
---


## notify {#notification}

Passes the specified notification object to the index to perform the notification.

```python
def notify(self, notification):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| notification | `Notification` | The notification object. |

**Returns:** bool: True if the notification was successfully performed; otherwise False.

### Example

```python
from groupdocs.search.common import Notification

notification = Notification.create_rename_notification(old_document_path, new_document_path)
result = index.notify(notification)
print("Notification applied:", result)
```

### Aliases

These names call `notify` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `notify_notification` | `notify_notification(notification)` |

### See Also
* class [`Index`](/search/python-net/groupdocs.search/index/)
