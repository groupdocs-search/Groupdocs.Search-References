---
title: "OperationType"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示索引操作类型。"
type: docs
weight: 23
url: /zh/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

表示索引操作类型。

## Fields

| Field | 描述 |
| --- | --- |
|  | [Indexing](#Indexing) | 向索引添加文档。 |
|
|  | [Updating](#Updating) | 更新索引中的文档。 |
|
|  | [Merging](#Merging) | 合并索引。 |
|
|  | [Optimizing](#Optimizing) | 优化索引。 |
|
|  | [Deleting](#Deleting) | 从索引中删除路径。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


向索引添加文档。


### Updating {#Updating}
```
public static final OperationType Updating
```


更新索引中的文档。


### Merging {#Merging}
```
public static final OperationType Merging
```


合并索引。


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


优化索引。


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


从索引中删除路径。


### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
