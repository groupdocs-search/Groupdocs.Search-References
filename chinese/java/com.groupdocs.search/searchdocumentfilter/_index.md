---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "包含用于创建搜索文档过滤器的方法。"
type: docs
weight: 24
url: /zh/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

包含用于创建搜索文档过滤器的方法。


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | 创建一个过滤器，用于跳过不匹配正则表达式的文档。 |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | 创建一个过滤器，用于跳过不匹配正则表达式的文档。 |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | 创建一个过滤器，用于跳过不在指定可能扩展名列表中的文档。 |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | 创建一个过滤器，其逻辑与指定的内部过滤器相反。 |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | 创建指定过滤器的逻辑合取。 |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | 创建指定过滤器的逻辑或运算。 |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | 创建一个过滤器，用于跳过不具备指定允许属性列表中任意值的文档。 |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


创建一个过滤器，用于跳过不匹配正则表达式的文档。正则表达式应用于文档的完整路径。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pattern | java.lang.String | 正则表达式模式。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
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
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


创建一个过滤器，用于跳过不在指定可能扩展名列表中的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | extensions | java.lang.String[] | 可能的扩展列表。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


创建一个过滤器，其逻辑与指定的内部过滤器相反。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | 内部搜索文档过滤器。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


创建指定过滤器的逻辑合取。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | 搜索文档过滤器。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


创建指定过滤器的逻辑或运算。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | 搜索文档过滤器。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


创建一个过滤器，用于跳过不具备指定允许属性列表中任意值的文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 属性 | java.lang.String[] | 允许的属性列表。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

