---
title: "SynonymDictionary"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mendefinisikan antarmuka kamus sinonim."
type: docs
weight: 23
url: /id/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Mendefinisikan antarmuka kamus sinonim.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCount()](#getCount--) | Mendapatkan jumlah kata yang terdapat dalam SynonymDictionary ini. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Menambahkan koleksi grup sinonim yang ditentukan ke instance SynonymDictionary ini. |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Menambahkan koleksi grup sinonim yang ditentukan ke instance SynonymDictionary ini. |
|
|  | [clear()](#clear--) | Menghapus semua kata dari objek SynonymDictionary ini. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Mendapatkan sinonim untuk kata yang ditentukan. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Mendapatkan semua grup sinonim yang dimiliki oleh kata yang ditentukan. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Mendapatkan semua grup sinonim yang terdapat dalam kamus ini. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator yang mengiterasi koleksi. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Mendapatkan jumlah kata yang terdapat dalam SynonymDictionary ini.


**Returns:**
int - Jumlah kata yang terdapat dalam SynonymDictionary ini.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Menambahkan koleksi grup sinonim yang ditentukan ke instance SynonymDictionary ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | sinonim | java.lang.Iterable<java.lang.String[]> | Koleksi grup sinonim untuk ditambahkan ke kamus. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Menambahkan koleksi grup sinonim yang ditentukan ke instance SynonymDictionary ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | sinonim | java.lang.String[][] | Koleksi grup sinonim untuk ditambahkan ke kamus. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Menghapus semua kata dari objek SynonymDictionary ini.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Mendapatkan sinonim untuk kata yang ditentukan. Array hasil tidak mengandung kata asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.String | Kata untuk menyarankan sinonim. |
|

**Returns:**
java.lang.String[] - Sinonim untuk kata yang ditentukan atau array kosong jika objek SynonymDictionary tidak mengandung kata yang dimaksud.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Mendapatkan semua grup sinonim yang dimiliki oleh kata yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.String | Kata untuk mendapatkan kelompok sinonim. |
|

**Returns:**
java.lang.String[][] - Semua kelompok sinonim yang dimiliki oleh kata yang ditentukan.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Mendapatkan semua grup sinonim yang terdapat dalam kamus ini.


**Returns:**
java.lang.String[][] - Semua kelompok sinonim.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Mengembalikan iterator yang mengiterasi koleksi.


**Returns:**
java.util.Iterator<java.lang.String> - Iterator yang dapat digunakan untuk mengiterasi koleksi.

