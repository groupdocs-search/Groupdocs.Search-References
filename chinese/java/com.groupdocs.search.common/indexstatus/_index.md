---
title: "IndexStatus"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "指定索引状态。"
type: docs
weight: 41
url: /zh/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

指定索引状态。

## Fields

| Field | 描述 |
| --- | --- |
|  | [Ready](#Ready) | 索引空闲且准备好进行更改。 |
|
|  | [Failed](#Failed) | 由于错误，索引需要重新加载。 |
|
|  | [Indexing](#Indexing) | 索引执行索引操作。 |
|
|  | [Updating](#Updating) | 索引执行更新操作。 |
|
|  | [Merging](#Merging) | 索引执行合并操作。 |
|
|  | [Optimizing](#Optimizing) | 索引执行优化操作。 |
|
|  | [Deleting](#Deleting) | 索引执行删除操作。 |
|
|  | [Renaming](#Renaming) | 索引执行重命名操作。 |
|
|  | [ChangingAttributes](#ChangingAttributes) | 索引更改属性。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


索引空闲且准备好进行更改。


### Failed {#Failed}
```
public static final IndexStatus Failed
```


由于错误，索引需要重新加载。


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


索引执行索引操作。


### Updating {#Updating}
```
public static final IndexStatus Updating
```


索引执行更新操作。


### Merging {#Merging}
```
public static final IndexStatus Merging
```


索引执行合并操作。


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


索引执行优化操作。


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


索引执行删除操作。


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


索引执行重命名操作。


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


索引更改属性。


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
