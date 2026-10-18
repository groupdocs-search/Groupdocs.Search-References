---
title: "Dokumen"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili kelas dasar untuk dokumen yang ditambahkan ke indeks dari aliran sistem file atau struktur."
type: docs
weight: 13
url: /id/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Mewakili kelas dasar untuk dokumen yang ditambahkan ke indeks dari sistem file, aliran, atau struktur. Berisi metode statis untuk membuat dokumen dari berbagai jenis sumber.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Mendapatkan jenis sumber dokumen. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Mendapatkan kunci dokumen yang digunakan untuk mengidentifikasi dokumen dalam indeks. |
|
|  | [isLazy()](#isLazy--) | Mendapatkan nilai yang menunjukkan apakah dokumen dimuat sesuai kebutuhan atau tidak. |
|
|  | [getModificationDate()](#getModificationDate--) | Mendapatkan tanggal modifikasi terakhir dokumen. |
|
|  | [getExtension()](#getExtension--) | Mendapatkan ekstensi yang digunakan untuk tipe dokumen ini. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Mendapatkan bidang tambahan untuk dokumen. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Mengatur bidang tambahan untuk dokumen. |
|
|  | [getAttributes()](#getAttributes--) | Mendapatkan atribut dokumen. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Mengatur atribut dokumen. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Membuat dokumen dari sebuah file. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Membuat dokumen dari sebuah aliran. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Membuat dokumen dari sebuah struktur yang merupakan array bidang teks. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Membuat dokumen yang dimuat secara malas. |
|
|  | [toString()](#toString--) | Mengembalikan  java.lang.String  yang mewakili  Document  saat ini. |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Mendapatkan jenis sumber dokumen.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Mendapatkan kunci dokumen yang digunakan untuk mengidentifikasi dokumen dalam indeks.


**Returns:**
java.lang.String - Kunci dokumen yang digunakan untuk mengidentifikasi dokumen dalam indeks.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Mendapatkan nilai yang menunjukkan apakah dokumen dimuat sesuai kebutuhan atau tidak.


**Returns:**
boolean - Nilai yang menunjukkan apakah dokumen dimuat sesuai kebutuhan atau tidak.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Mendapatkan tanggal modifikasi terakhir dokumen.


**Returns:**
java.util.Date - Tanggal modifikasi terakhir dokumen.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Mendapatkan ekstensi yang digunakan untuk tipe dokumen ini.


**Returns:**
java.lang.String - Ekstensi yang digunakan untuk tipe dokumen ini.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Mendapatkan bidang tambahan untuk dokumen.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Bidang tambahan untuk dokumen.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Mengatur bidang tambahan untuk dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Bidang tambahan untuk dokumen. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Mendapatkan atribut dokumen.


**Returns:**
java.lang.String[] - Atribut dokumen.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Mengatur atribut dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String[] | Atribut dokumen. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Membuat dokumen dari sebuah file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Path file dokumen. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Membuat dokumen dari sebuah aliran.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentKey | java.lang.String | Kunci dokumen. |
|
|  | modificationDate | java.util.Date | Tanggal modifikasi dokumen. |
|
|  | extension | java.lang.String | Ekstensi dokumen. |
|
|  | stream | java.io.InputStream | Stream dokumen. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Membuat dokumen dari sebuah struktur yang merupakan array bidang teks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentKey | java.lang.String | Kunci dokumen. |
|
|  | modificationDate | java.util.Date | Tanggal modifikasi dokumen. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Bidang dokumen. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Membuat dokumen yang dimuat secara malas.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | Jenis sumber dokumen. Nilai ini harus cocok dengan jenis dokumen yang dimuat. |
|
|  | documentKey | java.lang.String | Kunci dokumen. Nilai ini harus cocok dengan kunci dokumen yang dimuat. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | Pemuat dokumen. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Mengembalikan  java.lang.String  yang mewakili  Document  saat ini.


**Returns:**
java.lang.String - Sebuah java.lang.String yang mewakili Document saat ini.

