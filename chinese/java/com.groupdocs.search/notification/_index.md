---
title: "通知"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "索引所有通知的基类。"
type: docs
weight: 22
url: /zh/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

该类是所有针对索引的通知的基类。此类还包含用于创建通知对象的方法。


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Notification()](#Notification--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | 创建一个通知对象，用于重命名已被重命名且不需要重新索引的已索引文档。 |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


创建一个通知对象，用于重命名已被重命名且不需要重新索引的已索引文档。即使其内容已更改，重命名的文档在下一次更新操作中也不会被重新索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | oldPath | java.lang.String | 已索引文档的旧路径。 |
|
|  | newPath | java.lang.String | 已索引文档的新路径。 |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

