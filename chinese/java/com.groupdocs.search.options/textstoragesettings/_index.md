---
title: "TextStorageSettings"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示文本存储设置。"
type: docs
weight: 42
url: /zh/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

表示文本存储设置。


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | 初始化 TextStorageSettings 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCompression()](#getCompression--) | 获取文本存储的压缩。 |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | 设置文本存储的压缩。 |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


初始化 TextStorageSettings 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | 文本存储的压缩。 |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


获取文本存储的压缩。默认值为 Compression.Normal。


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


设置文本存储的压缩。默认值为 Compression.Normal。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | 文本存储的压缩。 |
|

