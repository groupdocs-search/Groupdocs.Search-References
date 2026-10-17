---
title: "FileIndexingEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث بدء فهرسة المستند."
type: docs
weight: 14
url: /ar/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

يمثل المعلمات لحدث بدء فهرسة المستند.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDocument()](#getDocument--) | يحصل على المستند. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | يحصل على المسار الكامل للمستند. |
|
|  | [getDocumentKey()](#getDocumentKey--) | يحصل على مفتاح المستند. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | يحصل على قيمة تشير إلى أنه يجب تخطي فهرسة المستند. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | يضبط قيمة تشير إلى أنه يجب تخطي فهرسة المستند. |
|
|  | [getEncoding()](#getEncoding--) | يحصل على ترميز المستند. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | يضبط ترميز المستند. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | يحصل على مستخرج النص المخصص. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | يضبط مستخرج النص المخصص. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | يحصل على الحقول الإضافية للمستند. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | يضبط الحقول الإضافية للمستند. |
|
|  | [getAttributes()](#getAttributes--) | يحصل على سمات المستند. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | اضبط سمات المستند. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


يحصل على المستند.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


يحصل على المسار الكامل للمستند.


**Returns:**
java.lang.String - المسار الكامل للمستند.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


يحصل على مفتاح المستند.


**Returns:**
java.lang.String - مفتاح المستند.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


يحصل على قيمة تشير إلى أنه يجب تخطي فهرسة المستند.


**Returns:**
boolean - قيمة تشير إلى أنه يجب تخطي فهرسة المستند.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


يضبط قيمة تشير إلى أنه يجب تخطي فهرسة المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى أنه يجب تخطي فهرسة المستند. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


يحصل على ترميز المستند.


**Returns:**
java.lang.String - ترميز المستند.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


يضبط ترميز المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String | ترميز المستند. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


يحصل على مستخرج النص المخصص.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


يضبط مستخرج النص المخصص.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | المستخرج النصي المخصص. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


يحصل على الحقول الإضافية للمستند.


**Returns:**
com.groupdocs.search.common.DocumentField[] - الحقول الإضافية للمستند.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


يضبط الحقول الإضافية للمستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | الحقول الإضافية للمستند. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


يحصل على سمات المستند.


**Returns:**
java.lang.String[] - سمات المستند.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


اضبط سمات المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String[] | سمات المستند. |
|

