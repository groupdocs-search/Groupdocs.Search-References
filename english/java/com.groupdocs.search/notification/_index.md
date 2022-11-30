---
title: Notification
second_title: GroupDocs.Search for Java API Reference
description: The base class for all notifications to the index.
type: docs
weight: 23
url: /java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

The base class for all notifications to the index. This class also contains methods for creating notification objects.

**Learn more**

 *  [Document renaming][]


[Document renaming]: https://docs.groupdocs.com/display/searchjava/Document+renaming
## Constructors

| Constructor | Description |
| --- | --- |
| [Notification()](#Notification--) |  |
## Methods

| Method | Description |
| --- | --- |
| [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Creates a notification object to rename an indexed document that has been renamed and does not need to be reindexed. |
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Creates a notification object to rename an indexed document that has been renamed and does not need to be reindexed. The renamed document will not be reindexed during the next update operation, even if its contents have been changed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldPath | java.lang.String | The old path to the indexed document. |
| newPath | java.lang.String | The new path to the indexed document. |

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.
