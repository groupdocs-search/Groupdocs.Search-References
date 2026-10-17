---
title: "DocumentInfo"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل وصفًا لوثيقة مفهرسة."
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

يمثل وصفًا لوثيقة مفهرسة.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [toString()](#toString--) | يرجع  System.String  الذي يمثل الـ DocumentInfo الحالي. |
|
|  | [getFilePath()](#getFilePath--) | يحصل على مسار الملف المفهرس من ملف أو مفتاح المستند المفهرس من تدفق أو بنية. |
|
|  | [getFileType()](#getFileType--) | يحصل على نوع الملف. |
|
|  | [getFormatFamily()](#getFormatFamily--) | يسترجع عائلة تنسيق المستند. |
|
|  | [getInnerPath()](#getInnerPath--) | يحصل على المسار الداخلي لعنصر المستند الحاوي. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | يحصل على أجزاء المسار الداخلي لعنصر المستند الحاوي. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | يحصل على نوع مصدر المستند. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | يحصل على مؤشر خطأ الفهرسة. |
|
|  | [serialize()](#serialize--) | يسلسل المثيل الحالي إلى مصفوفة بايت. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | يفك تسلسل مثيل من مصفوفة بايت. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


يرجع  System.String  الذي يمثل الـ DocumentInfo الحالي.


**Returns:**
java.lang.String -  System.String  الذي يمثل الـ DocumentInfo الحالي.

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


يحصل على مسار الملف المفهرس من ملف أو مفتاح المستند المفهرس من تدفق أو بنية.


**Returns:**
java.lang.String - مسار الملف أو مفتاح المستند.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


يحصل على نوع الملف.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


يسترجع عائلة تنسيق المستند.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


يحصل على المسار الداخلي لعنصر المستند الحاوي.


**Returns:**
java.lang.String - المسار الداخلي.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


يحصل على أجزاء المسار الداخلي لعنصر المستند الحاوي.


**Returns:**
java.lang.String[] - أجزاء المسار الداخلي.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


يحصل على نوع مصدر المستند.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


يحصل على مؤشر خطأ الفهرسة.


**Returns:**
boolean - مؤشر خطأ الفهرسة.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


يسلسل المثيل الحالي إلى مصفوفة بايت.


**Returns:**
byte[] - مصفوفة بايت تمثل المثيل الحالي.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


يفك تسلسل مثيل من مصفوفة بايت.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | مصفوفة | byte[] | مصفوفة بايت للتسلسل العكسي منها. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

