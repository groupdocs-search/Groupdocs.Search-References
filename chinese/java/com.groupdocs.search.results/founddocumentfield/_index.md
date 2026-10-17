---
title: "FoundDocumentField"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示已找到的文档字段。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

表示已找到的文档字段。


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | 获取字段名称。 |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 获取找到的出现次数。 |
|
|  | [getTerms()](#getTerms--) | 获取找到的词项。 |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | 获取已找到词项的出现次数。 |
|
|  | [getTermSequences()](#getTermSequences--) | 获取找到的词项序列。 |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | 获取已找到词项序列的出现次数。 |
|
|  | [toString()](#toString--) | 返回找到的文档字段的字符串表示。 |
|
|  | [serialize()](#serialize--) | 将当前实例序列化为字节数组。 |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | 从字节数组反序列化实例。 |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


获取字段名称。


**Returns:**
java.lang.String - 字段名称。

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


获取找到的出现次数。


**Returns:**
int - 已找到的出现次数。

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


获取找到的词项。


**Returns:**
java.lang.String[] - 已找到的词项。

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


获取已找到词项的出现次数。


**Returns:**
int[] - 已找到词项的出现次数。

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


获取找到的词项序列。


**Returns:**
java.lang.String[][] - 已找到的词项序列。

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


获取已找到词项序列的出现次数。


**Returns:**
int[] - 已找到词项序列的出现次数。

### toString() {#toString--}
```
public abstract String toString()
```


返回找到的文档字段的字符串表示。


**Returns:**
java.lang.String - 表示找到的文档字段的字符串。

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


将当前实例序列化为字节数组。


**Returns:**
byte[] - 表示当前实例的字节数组。

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


从字节数组反序列化实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数组 | byte[] | 用于反序列化的字节数组。 |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

