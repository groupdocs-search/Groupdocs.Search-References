---
title: "FoundDocument"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示已找到的文档。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

表示已找到的文档。


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | 获取文档信息。 |
|
|  | [getRelevance()](#getRelevance--) | 获取搜索结果的相关性。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 获取找到的出现次数。 |
|
|  | [getFoundFields()](#getFoundFields--) | 获取找到的文档字段。 |
|
|  | [getTerms()](#getTerms--) | 获取找到的词项。 |
|
|  | [getTermSequences()](#getTermSequences--) | 获取找到的词项序列。 |
|
|  | [getAttributes()](#getAttributes--) | 获取与找到的文档关联的属性。 |
|
|  | [toString()](#toString--) | 返回找到的文档的字符串表示。 |
|
|  | [serialize()](#serialize--) | 将当前实例序列化为字节数组。 |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | 从字节数组反序列化实例。 |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


获取文档信息。


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


获取搜索结果的相关性。


**Returns:**
double - 搜索结果的相关性。

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


获取找到的出现次数。


**Returns:**
int - 已找到的出现次数。

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


获取找到的文档字段。


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - 找到的文档字段。

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


获取找到的词项。每次访问属性时都会评估该值。


**Returns:**
java.lang.String[] - 已找到的词项。

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


获取找到的词项序列。


**Returns:**
java.lang.String[][] - 已找到的词项序列。

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


获取与找到的文档关联的属性。必须在搜索选项中启用相应的选项才能检索属性。


**Returns:**
java.lang.String[] - 与找到的文档关联的属性。

### toString() {#toString--}
```
public abstract String toString()
```


返回找到的文档的字符串表示。


**Returns:**
java.lang.String - 表示找到的文档的字符串。

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


将当前实例序列化为字节数组。


**Returns:**
byte[] - 表示当前实例的字节数组。

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


从字节数组反序列化实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数组 | byte[] | 用于反序列化的字节数组。 |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

