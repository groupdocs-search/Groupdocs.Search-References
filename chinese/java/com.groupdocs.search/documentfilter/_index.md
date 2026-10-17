---
title: "DocumentFilter"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示文档过滤器的基类。"
type: docs
weight: 14
url: /zh/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

表示文档过滤器的基类。包含用于创建文档过滤器实例的方法。


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [toString()](#toString--) | 返回文档过滤器的字符串表示。 |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | 创建一个过滤器，用于跳过创建日期早于下限的文档。 |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | 创建一个过滤器，用于跳过创建日期晚于上限的文档。 |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | 创建一个过滤器，用于跳过创建日期超出指定范围的文档。 |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | 创建一个过滤器，用于跳过修改日期早于下限的文档。 |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | 创建一个过滤器，用于跳过修改日期晚于上限的文档。 |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | 创建一个过滤器，用于跳过修改日期超出指定范围的文档。 |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | 创建一个过滤器，用于跳过不匹配正则表达式的文档。 |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | 创建一个过滤器，用于跳过不匹配正则表达式的文档。 |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | 创建一个过滤器，用于跳过长度小于下限的文档。 |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | 创建一个过滤器，用于跳过长度大于上限的文档。 |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | 创建一个过滤器，用于跳过超出指定文档长度范围的文档。 |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | 创建一个过滤器，用于跳过不具备允许扩展名的文档。 |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | 创建一个过滤器，其逻辑与指定的内部过滤器相反。 |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | 创建指定过滤器的逻辑合取。 |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | 创建指定过滤器的逻辑或运算。 |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


返回文档过滤器的字符串表示。


**Returns:**
java.lang.String - 文档过滤器的字符串表示。

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


创建一个过滤器，用于跳过创建日期早于下限的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | 文档创建时间的下限。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


创建一个过滤器，用于跳过创建日期晚于上限的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | upperBound | java.util.Date | 文档创建时间的上限。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


创建一个过滤器，用于跳过创建日期超出指定范围的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | 文档创建时间的下限。 |
|
|  | upperBound | java.util.Date | 文档创建时间的上限。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


创建一个过滤器，用于跳过修改日期早于下限的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | 文档修改时间的下限。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


创建一个过滤器，用于跳过修改日期晚于上限的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | upperBound | java.util.Date | 文档修改时间的上限。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


创建一个过滤器，用于跳过修改日期超出指定范围的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | 文档修改时间的下限。 |
|
|  | upperBound | java.util.Date | 文档修改时间的上限。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


创建一个过滤器，用于跳过不匹配正则表达式的文档。正则表达式应用于文档的完整路径。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pattern | java.lang.String | 正则表达式模式。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


创建一个过滤器，用于跳过不匹配正则表达式的文档。正则表达式应用于文档的完整路径。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pattern | java.lang.String | 正则表达式模式。 |
|
|  | options | int | 正则表达式选项。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


创建一个过滤器，用于跳过长度小于下限的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | lowerBound | long | 文档长度的下限。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


创建一个过滤器，用于跳过长度大于上限的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | upperBound | long | 文档长度的上限。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


创建一个过滤器，用于跳过超出指定文档长度范围的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | lowerBound | long | 文档长度的下限。 |
|
|  | upperBound | long | 文档长度的上限。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


创建一个过滤器，用于跳过不具备允许扩展名的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | extensions | java.lang.String[] | 允许的扩展名列表。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


创建一个过滤器，其逻辑与指定的内部过滤器相反。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | 内部文档过滤器。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


创建指定过滤器的逻辑合取。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | 文档过滤器。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


创建指定过滤器的逻辑或运算。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | 文档过滤器。 |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

