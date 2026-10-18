---
title: "StopWordDictionary"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mendefinisikan antarmuka kamus kata berhenti."
type: docs
weight: 22
url: /id/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Mendefinisikan antarmuka kamus kata berhenti.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCount()](#getCount--) | Mendapatkan jumlah stop word yang terkandung dalam StopWordDictionary. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Menambahkan koleksi kata yang ditentukan ke instance ini dari StopWordDictionary. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Menambahkan koleksi kata yang ditentukan ke instance ini dari StopWordDictionary. |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Menghapus koleksi kata yang ditentukan dari instance ini dari StopWordDictionary. |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Menghapus koleksi kata yang ditentukan dari instance ini dari StopWordDictionary. |
|
|  | [contains(String word)](#contains-java.lang.String-) | Menentukan apakah objek StopWordDictionary berisi kata yang ditentukan. |
|
|  | [clear()](#clear--) | Menghapus semua kata dari objek StopWordDictionary. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator yang mengiterasi koleksi. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Mendapatkan jumlah stop word yang terkandung dalam StopWordDictionary.


**Returns:**
int - Jumlah stop word dalam kamus.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Menambahkan koleksi kata yang ditentukan ke instance ini dari StopWordDictionary.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.Iterable<java.lang.String> | Koleksi kata untuk ditambahkan ke kamus. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Menambahkan koleksi kata yang ditentukan ke instance ini dari StopWordDictionary.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.String[] | Koleksi kata untuk ditambahkan ke kamus. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Menghapus koleksi kata yang ditentukan dari instance ini dari StopWordDictionary.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.Iterable<java.lang.String> | Koleksi kata untuk dihapus. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Menghapus koleksi kata yang ditentukan dari instance ini dari StopWordDictionary.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.String[] | Koleksi kata untuk dihapus. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Menentukan apakah objek StopWordDictionary berisi kata yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.String | Kata untuk dicari dalam objek StopWordDictionary. |
|

**Returns:**
boolean - true jika objek StopWordDictionary berisi kata yang ditentukan; jika tidak, false.

### clear() {#clear--}
```
public abstract void clear()
```


Menghapus semua kata dari objek StopWordDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Mengembalikan iterator yang mengiterasi koleksi.


**Returns:**
java.util.Iterator<java.lang.String> - Iterator yang dapat digunakan untuk mengiterasi koleksi.

