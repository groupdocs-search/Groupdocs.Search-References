---
title: "Compression"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "指定压缩级别。"
type: docs
weight: 47
url: /zh/java/com.groupdocs.search.options/compression/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum Compression extends Enum<Compression>
```

指定压缩级别。


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)

## Fields

| Field | 描述 |
| --- | --- |
|  | [None](#None) | 压缩已禁用。 |
|
|  | [Normal](#Normal) | 普通压缩级别。 |
|
|  | [High](#High) | 高压缩级别。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### None {#None}
```
public static final Compression None
```


压缩已禁用。


### Normal {#Normal}
```
public static final Compression Normal
```


普通压缩级别。


### High {#High}
```
public static final Compression High
```


高压缩级别。


### values() {#values--}
```
public static Compression[] values()
```




**Returns:**
com.groupdocs.search.options.Compression[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static Compression valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[Compression](../../com.groupdocs.search.options/compression)
