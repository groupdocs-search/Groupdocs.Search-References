---
title: "Compression"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "圧縮レベルを指定します。"
type: docs
weight: 47
url: /ja/java/com.groupdocs.search.options/compression/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum Compression extends Enum<Compression>
```

圧縮レベルを指定します。


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)

## Fields

| Field | 説明 |
| --- | --- |
|  | [None](#None) | 圧縮は無効です。 |
|
|  | [Normal](#Normal) | 標準圧縮レベルです。 |
|
|  | [High](#High) | 高圧縮レベルです。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### None {#None}
```
public static final Compression None
```


圧縮は無効です。


### Normal {#Normal}
```
public static final Compression Normal
```


標準圧縮レベルです。


### High {#High}
```
public static final Compression High
```


高圧縮レベルです。


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
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Compression](../../com.groupdocs.search.options/compression)
