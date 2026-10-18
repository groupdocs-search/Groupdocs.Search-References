---
title: "HomophoneDictionary"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mendefinisikan antarmuka kamus homofon heterografik."
type: docs
weight: 18
url: /id/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Mendefinisikan antarmuka kamus homofon heterografik.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCount()](#getCount--) | Mendapatkan jumlah kata yang terkandung dalam HomophoneDictionary ini. |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Menambahkan koleksi grup homofon yang ditentukan ke instance HomophoneDictionary ini. |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Menambahkan koleksi grup homofon yang ditentukan ke instance HomophoneDictionary ini. |
|
|  | [clear()](#clear--) | Menghapus semua kata dari objek HomophoneDictionary. |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Mendapatkan homofon untuk kata yang ditentukan. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Mendapatkan semua grup homofon yang dimiliki oleh kata yang ditentukan. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Mendapatkan semua grup homofon yang terkandung dalam kamus ini. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator yang mengiterasi koleksi. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Mendapatkan jumlah kata yang terkandung dalam HomophoneDictionary ini.


**Returns:**
int - Jumlah kata.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Menambahkan koleksi grup homofon yang ditentukan ke instance HomophoneDictionary ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | Koleksi grup homofon untuk ditambahkan ke kamus. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Menambahkan koleksi grup homofon yang ditentukan ke instance HomophoneDictionary ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | Koleksi grup homofon untuk ditambahkan ke kamus. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Menghapus semua kata dari objek HomophoneDictionary.


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Mendapatkan homofon untuk kata yang ditentukan. Array hasil tidak mengandung kata asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.String | Kata untuk menyarankan homofon. |
|

**Returns:**
java.lang.String[] - Homofon untuk kata yang ditentukan atau array kosong jika objek HomophoneDictionary tidak berisi kata yang ditentukan.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Mendapatkan semua grup homofon yang dimiliki oleh kata yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.String | Kata untuk mendapatkan grup homofon. |
|

**Returns:**
java.lang.String[][] - Semua grup homofon yang mana kata yang ditentukan termasuk.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Mendapatkan semua grup homofon yang terkandung dalam kamus ini.


**Returns:**
java.lang.String[][] - Semua grup homofon.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Mengembalikan iterator yang mengiterasi koleksi.


**Returns:**
java.util.Iterator<java.lang.String> - Iterator yang dapat digunakan untuk mengiterasi koleksi.

