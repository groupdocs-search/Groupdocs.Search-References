---
title: "DateFormatCollection"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili koleksi objek DateFormat."
type: docs
weight: 14
url: /id/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Mewakili koleksi objek DateFormat.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Menambahkan objek format tanggal ke koleksi. |
|
|  | [clear()](#clear--) | Menghapus semua elemen dari koleksi. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Menentukan apakah koleksi berisi item tertentu. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Menyalin elemen koleksi ke sebuah  Array , mulai dari indeks  Array  tertentu. |
|
|  | [size()](#size--) | Mendapatkan jumlah elemen yang terdapat dalam koleksi. |
|
|  | [isReadOnly()](#isReadOnly--) | Mendapatkan nilai yang menunjukkan apakah koleksi bersifat read-only. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Menghapus kemunculan pertama dari elemen tertentu dari koleksi. |
|
|  | [iterator()](#iterator--) | Mengembalikan enumerator yang mengiterasi koleksi. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Menambahkan objek format tanggal ke koleksi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Objek format tanggal yang akan ditambahkan ke koleksi. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Menghapus semua elemen dari koleksi.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Menentukan apakah koleksi berisi item tertentu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Item yang akan dicari dalam koleksi. |
|

**Returns:**
boolean -  true  jika item ditemukan dalam koleksi; jika tidak,  false .

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Menyalin elemen koleksi ke sebuah  Array , mulai dari indeks  Array  tertentu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | Array satu dimensi yang menjadi tujuan elemen yang disalin dari koleksi. |
|
|  | arrayIndex | int | Indeks berbasis nol dalam array tempat penyalinan dimulai. |
|

### size() {#size--}
```
public abstract int size()
```


Mendapatkan jumlah elemen yang terdapat dalam koleksi.


**Returns:**
int - Jumlah elemen yang terdapat dalam koleksi.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Mendapatkan nilai yang menunjukkan apakah koleksi bersifat read-only.


**Returns:**
boolean -  true  jika koleksi bersifat hanya-baca; jika tidak,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Menghapus kemunculan pertama dari elemen tertentu dari koleksi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Item yang akan dihapus dari koleksi. |
|

**Returns:**
boolean -  true  jika item berhasil dihapus dari koleksi; jika tidak,  false . Metode ini juga mengembalikan  false  jika item tidak ditemukan dalam koleksi.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Mengembalikan enumerator yang mengiterasi koleksi.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - Enumerator yang dapat digunakan untuk mengiterasi koleksi.

