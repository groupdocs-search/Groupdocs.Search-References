---
title: "CustomExtractorCollection"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Berisi kumpulan ekstraktor khusus."
type: docs
weight: 13
url: /id/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Berisi koleksi ekstraktor khusus. Jika koleksi berisi ekstraktor untuk beberapa ekstensi file yang sudah ditangani oleh ekstraktor bawaan, maka ekstraktor ini akan digunakan alih-alih yang bawaan.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [size()](#size--) | Mendapatkan jumlah ekstraktor yang terdapat dalam koleksi. |
|
|  | [isReadOnly()](#isReadOnly--) | Mendapatkan nilai yang menunjukkan apakah koleksi bersifat read-only. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator untuk koleksi ini. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Menambahkan ekstraktor ke koleksi. |
|
|  | [clear()](#clear--) | Menghapus semua ekstraktor dari koleksi. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Menentukan apakah koleksi berisi ekstraktor tertentu. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Menyalin elemen koleksi ke dalam array, dimulai pada indeks array tertentu. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Menghapus ekstraktor dari koleksi. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Mendapatkan jumlah ekstraktor yang terdapat dalam koleksi.


**Returns:**
int - Jumlah ekstraktor yang terdapat dalam koleksi.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Mendapatkan nilai yang menunjukkan apakah koleksi bersifat read-only.


**Returns:**
boolean - Nilai yang menunjukkan apakah koleksi bersifat hanya-baca.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Mengembalikan iterator untuk koleksi ini.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - Objek iterator yang dapat digunakan untuk mengiterasi koleksi.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Menambahkan ekstraktor ke koleksi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ekstraktor yang akan ditambahkan ke koleksi. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Menghapus semua ekstraktor dari koleksi.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Menentukan apakah koleksi berisi ekstraktor tertentu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ekstraktor yang akan dicari dalam koleksi. |
|

**Returns:**
boolean -  true  jika  item  ditemukan dalam koleksi; jika tidak,  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Menyalin elemen koleksi ke dalam array, dimulai pada indeks array tertentu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | Array satu dimensi yang menjadi tujuan elemen yang disalin dari koleksi. Array harus menggunakan indeks berbasis nol. |
|
|  | arrayIndex | int | Indeks berbasis nol dalam array tempat penyalinan dimulai. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Menghapus ekstraktor dari koleksi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Ekstraktor yang akan dihapus dari koleksi. |
|

**Returns:**
boolean -  true  jika  ekstraktor  berhasil dihapus dari koleksi; jika tidak,  false . Metode ini juga mengembalikan  false  jika  ekstraktor  tidak ditemukan dalam koleksi asli.

