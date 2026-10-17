---
title: "ImageSearchOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لعملية البحث العكسي عن الصور."
type: docs
weight: 24
url: /ar/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

يوفر خيارات لعملية البحث العكسي عن الصور.

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | ينشئ مثيلاً جديداً من الفئة  ImageSearchOptions  class. |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | ينشئ مثيلاً جديداً من الفئة  ImageSearchOptions  class. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | يحصل على الحد الأقصى لعدد البتات غير المتطابقة في تجزئة الصورة. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | يضبط الحد الأقصى لعدد البتات غير المتطابقة في تجزئة الصورة. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | يحصل على الحد الأقصى لعدد الصور المكتشفة لطلب البحث العكسي عن صورة. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | يضبط الحد الأقصى لعدد الصور المكتشفة لطلب البحث العكسي عن صورة. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | يحصل على مرشح مستند البحث. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | يحصل أو يضبط مرشح مستند البحث. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


ينشئ مثيلاً جديداً من الفئة  ImageSearchOptions  class.


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


ينشئ مثيلاً جديداً من الفئة  ImageSearchOptions  class.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البيانات | java.lang.Object | البيانات المتسلسلة. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


يحصل على الحد الأقصى لعدد البتات غير المتطابقة في تجزئة الصورة. القيمة الافتراضية هي  5 .


**Returns:**
int - الحد الأقصى لعدد البتات غير المتطابقة في تجزئة الصورة.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


يضبط الحد الأقصى لعدد البتات غير المتطابقة في تجزئة الصورة. القيمة الافتراضية هي  5 .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد البتات غير المتطابقة في تجزئة الصورة. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


يحصل على الحد الأقصى لعدد الصور المكتشفة لطلب البحث العكسي عن صورة. القيمة الافتراضية هي  1000 .


**Returns:**
int - الحد الأقصى لعدد الصور المكتشفة لطلب البحث العكسي عن صورة.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


يضبط الحد الأقصى لعدد الصور المكتشفة لطلب البحث العكسي عن صورة. القيمة الافتراضية هي  1000 .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد الصور المكتشفة لطلب البحث العكسي عن صورة. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


يحصل على مرشح مستند البحث. يعمل SearchDocumentFilter على منطق الإدراج. استخدم الفئة GroupDocs.Search.Options.SearchDocumentFilter لإنشاء مثيلات مرشح مستند البحث. القيمة الافتراضية هي null، مما يعني أنه سيتم إرجاع جميع المستندات التي تم العثور عليها.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


يحصل أو يضبط مرشح مستند البحث. يعمل SearchDocumentFilter على منطق الإدراج. استخدم الفئة GroupDocs.Search.Options.SearchDocumentFilter لإنشاء مثيلات مرشح مستند البحث. القيمة الافتراضية هي null، مما يعني أنه سيتم إرجاع جميع المستندات التي تم العثور عليها.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | مرشح مستند البحث. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
