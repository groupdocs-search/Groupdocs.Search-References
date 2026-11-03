---
title: Notification class
second_title: GroupDocs.Search for Python via .NET API References
description: "The base class for all notifications to the index."
type: docs
url: /python-net/groupdocs.search.common/notification/
is_root: false
weight: 260
---


## Notification class

The base class for all notifications to the index. This class also contains methods for creating notification objects.

Learn more

- https://docs.groupdocs.com/search/python-net/document-renaming/

The Notification type exposes the following members:

### Methods
| Method | Description |
| :- | :- |
| [create_rename_notification](/search/python-net/groupdocs.search.common/notification/create_rename_notification/#old_path-new_path) | Creates a rename notification for an indexed document that has been renamed and should not be reindexed during the next update operation. |

### Example

```python
from groupdocs.search.common import Notification

old_document_path = "old.docx"
new_document_path = "new.docx"

notification = Notification.create_rename_notification(old_document_path, new_document_path)
result = index.notify(notification)
print("Notification applied:", result)
```

### See Also
* module [`groupdocs.search.common`](/search/python-net/groupdocs.search.common/)
