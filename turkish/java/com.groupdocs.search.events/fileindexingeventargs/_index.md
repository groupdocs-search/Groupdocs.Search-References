---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belge indeksleme başlangıcı olayının argümanlarını temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Belge indeksleme başlangıcı olayının argümanlarını temsil eder.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDocument()](#getDocument--) | Belgeyi alır. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Belgenin tam yolunu alır. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Belge anahtarını alır. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Belgenin indekslenmesinin atlanması gerektiğini gösteren bir değeri alır. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Belgenin indekslenmesinin atlanması gerektiğini gösteren bir değeri ayarlar. |
|
|  | [getEncoding()](#getEncoding--) | Belgenin kodlamasını alır. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Belgenin kodlamasını ayarlar. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Özel metin çıkarıcıyı alır. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Özel metin çıkarıcıyı ayarlar. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Belge için ek alanları alır. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Belge için ek alanları ayarlar. |
|
|  | [getAttributes()](#getAttributes--) | Belgenin özniteliklerini alır. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Belgenin özniteliklerini ayarla. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Belgeyi alır.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Belgenin tam yolunu alır.


**Returns:**
java.lang.String - Belgenin tam yolu.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Belge anahtarını alır.


**Returns:**
java.lang.String - Belge anahtarı.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Belgenin indekslenmesinin atlanması gerektiğini gösteren bir değeri alır.


**Returns:**
boolean - Belgenin indekslenmesinin atlanması gerektiğini gösteren bir değer.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Belgenin indekslenmesinin atlanması gerektiğini gösteren bir değeri ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Belgenin indekslenmesinin atlanması gerektiğini gösteren bir değer. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Belgenin kodlamasını alır.


**Returns:**
java.lang.String - Belgenin kodlaması.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Belgenin kodlamasını ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Belgenin kodlaması. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Özel metin çıkarıcıyı alır.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Özel metin çıkarıcıyı ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Özel metin çıkarıcı. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Belge için ek alanları alır.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Belge için ek alanlar.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Belge için ek alanları ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Belge için ek alanlar. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Belgenin özniteliklerini alır.


**Returns:**
java.lang.String[] - Belgenin öznitelikleri.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Belgenin özniteliklerini ayarla.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String[] | Belgenin öznitelikleri. |
|

