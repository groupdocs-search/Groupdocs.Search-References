---
title: "DocumentFilter"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili kelas dasar untuk filter dokumen."
type: docs
weight: 14
url: /id/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Mewakili kelas dasar untuk filter dokumen. Berisi metode untuk membuat instance filter dokumen.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [toString()](#toString--) | Mengembalikan representasi string dari filter dokumen. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Membuat filter untuk melewatkan dokumen dengan tanggal pembuatan lebih awal dari batas bawah. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Membuat filter untuk melewatkan dokumen dengan tanggal pembuatan lebih akhir dari batas atas. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Membuat filter untuk melewatkan dokumen dengan tanggal pembuatan di luar rentang yang ditentukan. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Membuat filter untuk melewatkan dokumen dengan tanggal modifikasi lebih awal dari batas bawah. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Membuat filter untuk melewatkan dokumen dengan tanggal modifikasi lebih akhir dari batas atas. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Membuat filter untuk melewatkan dokumen dengan tanggal modifikasi di luar rentang yang ditentukan. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Membuat filter untuk melewatkan dokumen yang tidak cocok dengan ekspresi reguler. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Membuat filter untuk melewatkan dokumen yang tidak cocok dengan ekspresi reguler. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Membuat filter untuk melewatkan dokumen dengan panjang kurang dari batas bawah. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Membuat filter untuk melewatkan dokumen dengan panjang lebih dari batas atas. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Membuat filter untuk melewatkan dokumen di luar rentang panjang dokumen yang ditentukan. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Membuat filter untuk melewatkan dokumen yang tidak memiliki ekstensi yang diizinkan. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Membuat filter yang memiliki logika invers terkait filter dalam yang ditentukan. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Membuat konjungsi logis dari filter yang ditentukan. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Membuat disjungsi logis dari filter yang ditentukan. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Mengembalikan representasi string dari filter dokumen.


**Returns:**
java.lang.String - Representasi string dari filter dokumen.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Membuat filter untuk melewatkan dokumen dengan tanggal pembuatan lebih awal dari batas bawah.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Batas bawah waktu pembuatan dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Membuat filter untuk melewatkan dokumen dengan tanggal pembuatan lebih akhir dari batas atas.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | upperBound | java.util.Date | Batas atas waktu pembuatan dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Membuat filter untuk melewatkan dokumen dengan tanggal pembuatan di luar rentang yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Batas bawah waktu pembuatan dokumen. |
|
|  | upperBound | java.util.Date | Batas atas waktu pembuatan dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Membuat filter untuk melewatkan dokumen dengan tanggal modifikasi lebih awal dari batas bawah.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Batas bawah waktu modifikasi dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Membuat filter untuk melewatkan dokumen dengan tanggal modifikasi lebih akhir dari batas atas.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | upperBound | java.util.Date | Batas atas waktu modifikasi dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Membuat filter untuk melewatkan dokumen dengan tanggal modifikasi di luar rentang yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Batas bawah waktu modifikasi dokumen. |
|
|  | upperBound | java.util.Date | Batas atas waktu modifikasi dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Membuat filter untuk melewatkan dokumen yang tidak cocok dengan ekspresi reguler. Ekspresi reguler diterapkan pada jalur lengkap dokumen.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pattern | java.lang.String | Pola ekspresi reguler. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
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
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Membuat filter untuk melewatkan dokumen dengan panjang kurang dari batas bawah.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lowerBound | long | Batas bawah panjang dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Membuat filter untuk melewatkan dokumen dengan panjang lebih dari batas atas.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | upperBound | long | Batas atas panjang dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Membuat filter untuk melewatkan dokumen di luar rentang panjang dokumen yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | lowerBound | long | Batas bawah panjang dokumen. |
|
|  | upperBound | long | Batas atas panjang dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Membuat filter untuk melewatkan dokumen yang tidak memiliki ekstensi yang diizinkan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Daftar ekstensi yang diizinkan. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Membuat filter yang memiliki logika invers terkait filter dalam yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Filter dokumen internal. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Membuat konjungsi logis dari filter yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Filter dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Membuat disjungsi logis dari filter yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Filter dokumen. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

