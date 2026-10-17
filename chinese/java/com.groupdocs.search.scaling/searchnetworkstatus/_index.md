---
title: "SearchNetworkStatus"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "指定搜索网络状态。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.search.scaling/searchnetworkstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchNetworkStatus extends Enum<SearchNetworkStatus>
```

指定搜索网络状态。

## Fields

| Field | 描述 |
| --- | --- |
|  | [Ready](#Ready) | 搜索网络是空闲的，已准备好进行更改。 |
|
|  | [Configuring](#Configuring) | 搜索网络执行配置操作。 |
|
|  | [Indexing](#Indexing) | 搜索网络执行索引操作。 |
|
|  | [Optimizing](#Optimizing) | 搜索网络执行优化操作。 |
|
|  | [Deleting](#Deleting) | 搜索网络执行删除操作。 |
|
|  | [ChangingAttributes](#ChangingAttributes) | 搜索网络更改属性。 |
|
|  | [Synchronizing](#Synchronizing) | 搜索网络执行同步操作。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final SearchNetworkStatus Ready
```


搜索网络是空闲的，已准备好进行更改。


### Configuring {#Configuring}
```
public static final SearchNetworkStatus Configuring
```


搜索网络执行配置操作。


### Indexing {#Indexing}
```
public static final SearchNetworkStatus Indexing
```


搜索网络执行索引操作。


### Optimizing {#Optimizing}
```
public static final SearchNetworkStatus Optimizing
```


搜索网络执行优化操作。


### Deleting {#Deleting}
```
public static final SearchNetworkStatus Deleting
```


搜索网络执行删除操作。


### ChangingAttributes {#ChangingAttributes}
```
public static final SearchNetworkStatus ChangingAttributes
```


搜索网络更改属性。


### Synchronizing {#Synchronizing}
```
public static final SearchNetworkStatus Synchronizing
```


搜索网络执行同步操作。


### values() {#values--}
```
public static SearchNetworkStatus[] values()
```




**Returns:**
com.groupdocs.search.scaling.SearchNetworkStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static SearchNetworkStatus valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus)
