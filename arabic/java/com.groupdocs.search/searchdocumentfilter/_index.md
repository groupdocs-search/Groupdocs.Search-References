---
title: "SearchDocumentFilter"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحتوي على طرق لإنشاء مرشحات مستندات البحث."
type: docs
weight: 24
url: /ar/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

يحتوي على طرق لإنشاء مرشحات مستندات البحث.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | ينشئ مرشحًا لتخطي المستندات التي لا تتطابق مع تعبير عادي. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | ينشئ مرشحًا لتخطي المستندات التي لا تتطابق مع تعبير عادي. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | ينشئ مرشحًا لتخطي المستندات التي ليست في القائمة المحددة للامتدادات الممكنة. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | ينشئ مرشحًا يمتلك منطقًا عكسيًا بالنسبة للمرشح الداخلي المحدد. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | ينشئ تقاطعًا منطقيًا للمرشحات المحددة. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | ينشئ اتحادًا منطقيًا للمرشحات المحددة. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | ينشئ مرشحًا لتخطي المستندات التي لا تحتوي على أي قيمة من القائمة المحددة للسمات المسموح بها. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


ينشئ مرشحًا لتخطي المستندات التي لا تتطابق مع تعبير عادي. يتم تطبيق التعبير العادي على المسار الكامل للمستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | pattern | java.lang.String | نمط التعبير العادي. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


ينشئ مرشحًا لتخطي المستندات التي لا تتطابق مع تعبير عادي. يتم تطبيق التعبير العادي على المسار الكامل للمستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | pattern | java.lang.String | نمط التعبير العادي. |
|
|  | options | int | خيارات التعبير العادي. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


ينشئ مرشحًا لتخطي المستندات التي ليست في القائمة المحددة للامتدادات الممكنة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | extensions | java.lang.String[] | قائمة الامتدادات الممكنة. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


ينشئ مرشحًا يمتلك منطقًا عكسيًا بالنسبة للمرشح الداخلي المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | المرشح الداخلي للبحث في المستندات. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


ينشئ تقاطعًا منطقيًا للمرشحات المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | مرشحات البحث في المستندات. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


ينشئ اتحادًا منطقيًا للمرشحات المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | مرشحات البحث في المستندات. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


ينشئ مرشحًا لتخطي المستندات التي لا تحتوي على أي قيمة من القائمة المحددة للسمات المسموح بها.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | attributes | java.lang.String[] | قائمة السمات المسموح بها. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

