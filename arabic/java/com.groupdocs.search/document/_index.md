---
title: "مستند"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل الفئة الأساسية للمستندات المضافة إلى الفهرس من تدفق نظام الملفات أو الهيكل."
type: docs
weight: 13
url: /ar/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

يمثل الفئة الأساسية للمستندات المضافة إلى الفهرس من نظام الملفات أو التدفق أو الهيكل. يحتوي على طرق ثابتة لإنشاء مستندات من أنواع مختلفة من المصادر.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | يحصل على نوع مصدر المستند. |
|
|  | [getDocumentKey()](#getDocumentKey--) | يحصل على مفتاح المستند المستخدم لتحديد المستند داخل الفهرس. |
|
|  | [isLazy()](#isLazy--) | يحصل على قيمة تشير إلى ما إذا كان المستند محملاً حسب الحاجة أم لا. |
|
|  | [getModificationDate()](#getModificationDate--) | يحصل على تاريخ التعديل الأخير للمستند. |
|
|  | [getExtension()](#getExtension--) | يحصل على الامتداد المستخدم لهذا النوع من المستندات. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | يحصل على الحقول الإضافية للمستند. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | يضبط الحقول الإضافية للمستند. |
|
|  | [getAttributes()](#getAttributes--) | يحصل على سمات المستند. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | يضبط سمات المستند. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | ينشئ مستندًا من ملف. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | ينشئ مستندًا من تدفق. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | ينشئ مستندًا من بنية هي مصفوفة من حقول النص. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | ينشئ مستندًا محملاً بشكل كسول. |
|
|  | [toString()](#toString--) | يرجع  java.lang.String  الذي يمثل الـ Document الحالي. |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


يحصل على نوع مصدر المستند.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


يحصل على مفتاح المستند المستخدم لتحديد المستند داخل الفهرس.


**Returns:**
java.lang.String - مفتاح المستند المستخدم لتحديد المستند داخل الفهرس.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


يحصل على قيمة تشير إلى ما إذا كان المستند محملاً حسب الحاجة أم لا.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان المستند محملاً حسب الحاجة أم لا.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


يحصل على تاريخ التعديل الأخير للمستند.


**Returns:**
java.util.Date - تاريخ التعديل الأخير للمستند.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


يحصل على الامتداد المستخدم لهذا النوع من المستندات.


**Returns:**
java.lang.String - الامتداد المستخدم لهذا النوع من المستندات.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


يحصل على الحقول الإضافية للمستند.


**Returns:**
com.groupdocs.search.common.DocumentField[] - الحقول الإضافية للمستند.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


يضبط الحقول الإضافية للمستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | الحقول الإضافية للمستند. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


يحصل على سمات المستند.


**Returns:**
java.lang.String[] - سمات المستند.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


يضبط سمات المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String[] | سمات المستند. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


ينشئ مستندًا من ملف.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار ملف المستند. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


ينشئ مستندًا من تدفق.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentKey | java.lang.String | مفتاح المستند. |
|
|  | modificationDate | java.util.Date | تاريخ تعديل المستند. |
|
|  | extension | java.lang.String | امتداد المستند. |
|
|  | stream | java.io.InputStream | تيار المستند. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


ينشئ مستندًا من بنية هي مصفوفة من حقول النص.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentKey | java.lang.String | مفتاح المستند. |
|
|  | modificationDate | java.util.Date | تاريخ تعديل المستند. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | حقول المستند. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


ينشئ مستندًا محملاً بشكل كسول.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | نوع مصدر المستند. يجب أن تتطابق هذه القيمة مع نوع المستند المحمَّل. |
|
|  | documentKey | java.lang.String | مفتاح المستند. يجب أن تتطابق هذه القيمة مع مفتاح المستند المحمَّل. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | محمل المستند. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


يرجع  java.lang.String  الذي يمثل الـ Document الحالي.


**Returns:**
java.lang.String - أ  java.lang.String  التي تمثل الـ Document الحالي.

