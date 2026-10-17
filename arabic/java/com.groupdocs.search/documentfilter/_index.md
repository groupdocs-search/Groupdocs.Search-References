---
title: "DocumentFilter"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل الفئة الأساسية لمرشحات المستندات."
type: docs
weight: 14
url: /ar/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

يمثل الفئة الأساسية لمرشحات المستندات. يحتوي على طرق لإنشاء مثيلات مرشح المستند.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [toString()](#toString--) | يرجع تمثيلًا نصيًا لمرشح المستند. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | ينشئ مرشحًا لتخطي المستندات التي تاريخ إنشائها أسبق الحد الأدنى. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | ينشئ مرشحًا لتخطي المستندات التي تاريخ إنشائها لاحقًا للحد الأعلى. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | ينشئ مرشحًا لتخطي المستندات التي تاريخ إنشائها خارج النطاق المحدد. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | ينشئ مرشحًا لتخطي المستندات التي تاريخ تعديلها أسبق الحد الأدنى. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | ينشئ مرشحًا لتخطي المستندات التي تاريخ تعديلها لاحقًا للحد الأعلى. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | ينشئ مرشحًا لتخطي المستندات التي تاريخ تعديلها خارج النطاق المحدد. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | ينشئ مرشحًا لتخطي المستندات التي لا تتطابق مع تعبير عادي. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | ينشئ مرشحًا لتخطي المستندات التي لا تتطابق مع تعبير عادي. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | ينشئ مرشحًا لتخطي المستندات التي طولها أقل من الحد الأدنى. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | ينشئ مرشحًا لتخطي المستندات التي طولها أكبر من الحد الأعلى. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | ينشئ مرشحًا لتخطي المستندات خارج نطاق طول المستند المحدد. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | ينشئ مرشحًا لتخطي المستندات التي لا تحتوي على امتداد مسموح به. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | ينشئ مرشحًا يمتلك منطقًا عكسيًا بالنسبة للمرشح الداخلي المحدد. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | ينشئ تقاطعًا منطقيًا للمرشحات المحددة. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | ينشئ اتحادًا منطقيًا للمرشحات المحددة. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


يرجع تمثيلًا نصيًا لمرشح المستند.


**Returns:**
java.lang.String - تمثيل نصي لمرشح المستند.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


ينشئ مرشحًا لتخطي المستندات التي تاريخ إنشائها أسبق الحد الأدنى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | lowerBound | java.util.Date | الحد الأدنى لوقت إنشاء المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


ينشئ مرشحًا لتخطي المستندات التي تاريخ إنشائها لاحقًا للحد الأعلى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | upperBound | java.util.Date | الحد الأعلى لوقت إنشاء المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


ينشئ مرشحًا لتخطي المستندات التي تاريخ إنشائها خارج النطاق المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | lowerBound | java.util.Date | الحد الأدنى لوقت إنشاء المستند. |
|
|  | upperBound | java.util.Date | الحد الأعلى لوقت إنشاء المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


ينشئ مرشحًا لتخطي المستندات التي تاريخ تعديلها أسبق الحد الأدنى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | lowerBound | java.util.Date | الحد الأدنى لوقت تعديل المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


ينشئ مرشحًا لتخطي المستندات التي تاريخ تعديلها لاحقًا للحد الأعلى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | upperBound | java.util.Date | الحد الأعلى لوقت تعديل المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


ينشئ مرشحًا لتخطي المستندات التي تاريخ تعديلها خارج النطاق المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | lowerBound | java.util.Date | الحد الأدنى لوقت تعديل المستند. |
|
|  | upperBound | java.util.Date | الحد الأعلى لوقت تعديل المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


ينشئ مرشحًا لتخطي المستندات التي لا تتطابق مع تعبير عادي. يتم تطبيق التعبير العادي على المسار الكامل للمستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | pattern | java.lang.String | نمط التعبير العادي. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
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
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


ينشئ مرشحًا لتخطي المستندات التي طولها أقل من الحد الأدنى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | lowerBound | long | الحد الأدنى لطول المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


ينشئ مرشحًا لتخطي المستندات التي طولها أكبر من الحد الأعلى.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | upperBound | long | الحد الأعلى لطول المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


ينشئ مرشحًا لتخطي المستندات خارج نطاق طول المستند المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | lowerBound | long | الحد الأدنى لطول المستند. |
|
|  | upperBound | long | الحد الأعلى لطول المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


ينشئ مرشحًا لتخطي المستندات التي لا تحتوي على امتداد مسموح به.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | extensions | java.lang.String[] | قائمة الامتدادات المسموح بها. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


ينشئ مرشحًا يمتلك منطقًا عكسيًا بالنسبة للمرشح الداخلي المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | مرشح المستند الداخلي. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


ينشئ تقاطعًا منطقيًا للمرشحات المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | مرشحات المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


ينشئ اتحادًا منطقيًا للمرشحات المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | مرشحات المستند. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

