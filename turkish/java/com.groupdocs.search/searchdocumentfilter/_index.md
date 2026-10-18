---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama belge filtreleri oluşturmak için yöntemler içerir."
type: docs
weight: 24
url: /tr/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Arama belge filtreleri oluşturmak için yöntemler içerir.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Bir düzenli ifadeye uymayan belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Bir düzenli ifadeye uymayan belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Belirtilen olası uzantıların listesinde olmayan belgeleri atlamak için bir filtre oluşturur. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Belirtilen iç filtreyle ilişkili ters mantığa sahip bir filtre oluşturur. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Belirtilen filtrelerin mantıksal birleşimini oluşturur. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Belirtilen filtrelerin mantıksal ayrımını oluşturur. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Belirtilen izin verilen öznitelik listesinde herhangi bir değere sahip olmayan belgeleri atlamak için bir filtre oluşturur. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Bir düzenli ifadeye uymayan belgeleri atlamak için bir filtre oluşturur. Düzenli ifade, bir belgenin tam yoluna uygulanır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pattern | java.lang.String | Düzenli ifade deseni. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Bir düzenli ifadeye uymayan belgeleri atlamak için bir filtre oluşturur. Düzenli ifade, bir belgenin tam yoluna uygulanır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pattern | java.lang.String | Düzenli ifade deseni. |
|
|  | options | int | Düzenli ifade seçenekleri. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Belirtilen olası uzantıların listesinde olmayan belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Olası uzantıların listesi. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Belirtilen iç filtreyle ilişkili ters mantığa sahip bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | İç arama belge filtresi. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Belirtilen filtrelerin mantıksal birleşimini oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Arama belge filtreleri. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Belirtilen filtrelerin mantıksal ayrımını oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Arama belge filtreleri. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Belirtilen izin verilen öznitelik listesinde herhangi bir değere sahip olmayan belgeleri atlamak için bir filtre oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | attributes | java.lang.String[] | İzin verilen özniteliklerin listesi. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

