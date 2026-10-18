---
title: "SearchDocumentFilter"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Berisi metode untuk membuat filter dokumen pencarian."
type: docs
weight: 24
url: /id/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Berisi metode untuk membuat filter dokumen pencarian.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Membuat filter untuk melewatkan dokumen yang tidak cocok dengan ekspresi reguler. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Membuat filter untuk melewatkan dokumen yang tidak cocok dengan ekspresi reguler. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Membuat filter untuk melewatkan dokumen yang tidak berada dalam daftar ekstensi yang mungkin ditentukan. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Membuat filter yang memiliki logika invers terkait filter dalam yang ditentukan. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Membuat konjungsi logis dari filter yang ditentukan. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Membuat disjungsi logis dari filter yang ditentukan. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Membuat filter untuk melewatkan dokumen yang tidak memiliki nilai apa pun dari daftar atribut yang diizinkan yang ditentukan. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Membuat filter untuk melewatkan dokumen yang tidak cocok dengan ekspresi reguler. Ekspresi reguler diterapkan pada jalur lengkap dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pattern | java.lang.String | Pola ekspresi reguler. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Membuat filter untuk melewatkan dokumen yang tidak cocok dengan ekspresi reguler. Ekspresi reguler diterapkan pada jalur lengkap dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pattern | java.lang.String | Pola ekspresi reguler. |
|
|  | options | int | Opsi ekspresi reguler. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Membuat filter untuk melewatkan dokumen yang tidak berada dalam daftar ekstensi yang mungkin ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Daftar ekstensi yang mungkin. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Membuat filter yang memiliki logika invers terkait filter dalam yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Filter dokumen pencarian internal. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Membuat konjungsi logis dari filter yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Filter dokumen pencarian. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Membuat disjungsi logis dari filter yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Filter dokumen pencarian. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Membuat filter untuk melewatkan dokumen yang tidak memiliki nilai apa pun dari daftar atribut yang diizinkan yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | atribut | java.lang.String[] | Daftar atribut yang diizinkan. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

