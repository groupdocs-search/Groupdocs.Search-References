---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "提供索引元数据字段的选项。"
type: docs
weight: 29
url: /zh/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

提供索引元数据字段的选项。


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | 获取一个值，指示是否对空字段值进行索引。 |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | 设置一个值，指示是否对空字段值进行索引。 |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | 获取一个值，指示是否对空字段名进行索引。 |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | 设置一个值，指示是否对空字段名进行索引。 |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | 获取用于索引空字段名的默认字段名。 |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | 设置用于索引空字段名的默认字段名。 |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | 获取字段复合名称中的分隔符。 |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | 设置字段复合名称中的分隔符。 |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | 获取用于索引字段的 byte 类型数组中的最大值数量。 |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | 设置用于索引字段的 byte 类型数组中的最大值数量。 |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | 获取用于索引字段的 int 类型数组中的最大值数量。 |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | 设置用于索引字段的 int 类型数组中的最大值数量。 |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | 获取用于索引字段的 long 类型数组中的最大值数量。 |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | 设置用于索引字段的 long 类型数组中的最大值数量。 |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | 获取用于索引字段的 double 类型数组中的最大值数量。 |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | 设置用于索引字段的 double 类型数组中的最大值数量。 |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | 获取数组类型字段中值之间的分隔符。 |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | 设置数组类型字段中值之间的分隔符。 |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


获取一个值，指示是否对空字段值进行索引。默认值为 true。


**Returns:**
布尔型 - 指示是否对空字段值进行索引的值。

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


设置一个指示是否索引空字段值的值。默认值为 true。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否索引空字段值的值。 |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


获取一个指示是否索引空字段名的值。默认值为 true。


**Returns:**
boolean - 指示是否索引空字段名的值。

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


设置一个指示是否索引空字段名的值。默认值为 true。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | boolean | 指示是否索引空字段名的值。 |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


获取用于索引空字段名的默认字段名。默认值为 \"unknown\"。


**Returns:**
java.lang.String - 用于索引空字段名的默认字段名。

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


设置用于索引空字段名的默认字段名。默认值为 \"unknown\"。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 用于索引空字段名的默认字段名。 |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


获取字段复合名称中的分隔符。默认值为 \".\"。


**Returns:**
java.lang.String - 字段复合名称中的分隔符。

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


设置字段复合名称中的分隔符。默认值为 \".\"。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 字段复合名称中的分隔符。 |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


获取用于索引字段的 byte 类型数组中的最大值数量。默认值为 Integer.MAX_VALUE。


**Returns:**
int - 用于索引字段的 byte 类型数组中的最大值数量。

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


设置用于索引字段的 byte 类型数组中的最大值数量。默认值为 Integer.MAX_VALUE。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 用于索引字段的 byte 类型数组中的最大值数量。 |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


获取用于索引字段的 int 类型数组中的最大值数量。默认值为 Integer.MAX_VALUE。


**Returns:**
int - 用于索引字段的 int 类型数组中的最大值数量。

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


设置用于索引字段的 int 类型数组中的最大值数量。默认值为 Integer.MAX_VALUE。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 用于索引字段的 int 类型数组中的最大值数量。 |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


获取用于索引字段的 long 类型数组中的最大值数量。默认值为 Integer.MAX_VALUE。


**Returns:**
int - 用于索引字段的 long 类型数组中的最大值数量。

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


设置用于索引字段的 long 类型数组中的最大值数量。默认值为 Integer.MAX_VALUE。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 用于索引字段的 long 类型数组的最大值数量。 |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


获取用于索引字段的 double 类型数组的最大值数量。默认值为 Integer.MAX_VALUE。


**Returns:**
int - 用于索引字段的 double 类型数组的最大值数量。

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


设置用于索引字段的 double 类型数组的最大值数量。默认值为 Integer.MAX_VALUE。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | 用于索引字段的 double 类型数组的最大值数量。 |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


获取类型为数组的字段中值之间的分隔符。默认值为空格符号。


**Returns:**
java.lang.String - 类型为数组的字段中值之间的分隔符。

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


设置类型为数组的字段中值之间的分隔符。默认值为空格符号。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 类型为数组的字段中值之间的分隔符。 |
|

