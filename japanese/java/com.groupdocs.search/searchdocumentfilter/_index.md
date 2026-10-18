---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "検索ドキュメントフィルタを作成するメソッドを含みます。"
type: docs
weight: 24
url: /ja/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

検索ドキュメントフィルタを作成するメソッドを含みます。


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | 正規表現に一致しないドキュメントをスキップするフィルターを作成します。 |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | 正規表現に一致しないドキュメントをスキップするフィルターを作成します。 |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | 指定された可能な拡張子のリストに含まれないドキュメントをスキップするフィルターを作成します。 |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | 指定された内部フィルターに対して逆のロジックを持つフィルターを作成します。 |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | 指定されたフィルターの論理積を作成します。 |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | 指定されたフィルターの論理和を作成します。 |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | 指定された許容属性リストのいずれの値も持たないドキュメントをスキップするフィルターを作成します。 |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


正規表現に一致しないドキュメントをスキップするフィルターを作成します。正規表現はドキュメントのフルパスに適用されます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パターン | java.lang.String | 正規表現パターンです。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


正規表現に一致しないドキュメントをスキップするフィルターを作成します。正規表現はドキュメントのフルパスに適用されます。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | パターン | java.lang.String | 正規表現パターンです。 |
|
|  | オプション | int | 正規表現のオプションです。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


指定された可能な拡張子のリストに含まれないドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 拡張子 | java.lang.String[] | 可能な拡張子のリストです。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


指定された内部フィルターに対して逆のロジックを持つフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | 内部検索ドキュメントフィルターです。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


指定されたフィルターの論理積を作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | 検索ドキュメントフィルターです。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


指定されたフィルターの論理和を作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | 検索ドキュメントフィルターです。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


指定された許容属性リストのいずれの値も持たないドキュメントをスキップするフィルターを作成します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 属性 | java.lang.String[] | 許容属性のリストです。 |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

