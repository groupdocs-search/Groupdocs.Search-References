---
title: "FileIndexingEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa ketika pengindeksan dokumen dimulai."
type: docs
weight: 14
url: /id/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Mewakili argumen untuk peristiwa ketika pengindeksan dokumen dimulai.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDocument()](#getDocument--) | Mendapatkan dokumen. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Mendapatkan jalur lengkap dokumen. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Mendapatkan kunci dokumen. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Mendapatkan nilai yang menunjukkan bahwa pengindeksan dokumen harus dilewati. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Mengatur nilai yang menunjukkan bahwa pengindeksan dokumen harus dilewati. |
|
|  | [getEncoding()](#getEncoding--) | Mendapatkan enkoding dokumen. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Mengatur enkoding dokumen. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Mendapatkan pengekstrak teks khusus. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Mengatur ekstraktor teks khusus. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Mendapatkan bidang tambahan untuk dokumen. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Mengatur bidang tambahan untuk dokumen. |
|
|  | [getAttributes()](#getAttributes--) | Mendapatkan atribut dokumen. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Atur atribut dokumen. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Mendapatkan dokumen.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Mendapatkan jalur lengkap dokumen.


**Returns:**
java.lang.String - Jalur lengkap dokumen.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Mendapatkan kunci dokumen.


**Returns:**
java.lang.String - Kunci dokumen.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Mendapatkan nilai yang menunjukkan bahwa pengindeksan dokumen harus dilewati.


**Returns:**
boolean - Nilai yang menunjukkan bahwa pengindeksan dokumen harus dilewati.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Mengatur nilai yang menunjukkan bahwa pengindeksan dokumen harus dilewati.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan bahwa pengindeksan dokumen harus dilewati. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Mendapatkan enkoding dokumen.


**Returns:**
java.lang.String - Enkoding dokumen.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Mengatur enkoding dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Enkoding dokumen. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Mendapatkan pengekstrak teks khusus.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Mengatur ekstraktor teks khusus.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Pengekstrak teks khusus. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Mendapatkan bidang tambahan untuk dokumen.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Bidang tambahan untuk dokumen.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Mengatur bidang tambahan untuk dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Bidang tambahan untuk dokumen. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Mendapatkan atribut dokumen.


**Returns:**
java.lang.String[] - Atribut dokumen.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Atur atribut dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String[] | Atribut dokumen. |
|

