---
title: create_rename_notification method
second_title: GroupDocs.Search for Python via .NET API References
description: "Creates a rename notification for an indexed document that has been renamed and should not be reindexed during the next update operation."
type: docs
url: /python-net/groupdocs.search.common/notification/create_rename_notification/
is_root: false
weight: 1010
---


## create_rename_notification {#old_path-new_path}

Creates a rename notification for an indexed document that has been renamed and should not be reindexed during the next update operation.

Sometimes a situation arises when an indexed document is renamed but its contents have not changed. Notifying the index about the rename saves computing resources because the document will not be reindexed during the update operation.

```python
def create_rename_notification(cls, old_path, new_path):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| old_path | `str` | The old path to the indexed document. |
| new_path | `str` | The new path to the indexed document. |

**Returns:** Notification: A new rename notification object.

### Example

```python
from groupdocs.search.common import Notification

old_document_path = "/docs/old_name.pdf"
new_document_path = "/docs/new_name.pdf"

notification = Notification.create_rename_notification(old_document_path, new_document_path)
result = index.notify(notification)
print("Notification applied:", result)
```

### See Also
* class [`Notification`](/search/python-net/groupdocs.search.common/notification/)
