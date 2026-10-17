---
title: "ExtractedData"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示从文档检索并准备进行索引的数据。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

表示从文档检索并准备进行索引的数据。

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [serialize()](#serialize--) | 将当前实例序列化为字节数组。 |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | 从字节数组反序列化实例。 |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


将当前实例序列化为字节数组。


**Returns:**
byte[] - 表示当前实例的字节数组。

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


从字节数组反序列化实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数组 | byte[] | 用于反序列化的字节数组。 |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

