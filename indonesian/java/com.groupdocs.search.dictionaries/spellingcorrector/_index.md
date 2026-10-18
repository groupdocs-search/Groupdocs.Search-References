---
title: "SpellingCorrector"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mendefinisikan antarmuka korektor ejaan untuk istilah dalam kueri."
type: docs
weight: 21
url: /id/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Mendefinisikan antarmuka korektor ejaan untuk istilah dalam kueri.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCount()](#getCount--) | Mendapatkan jumlah kata yang terdapat dalam SpellingCorrector ini. |
|
|  | [getWords()](#getWords--) | Mendapatkan koleksi kata yang saat ini terdapat dalam SpellingCorrector ini. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Menambahkan koleksi kata yang ditentukan ke instance ini dari SpellingCorrector. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Menambahkan koleksi kata yang ditentukan ke instance ini dari SpellingCorrector. |
|
|  | [clear()](#clear--) | Menghapus semua kata dari objek SpellingCorrector. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Mendapatkan jumlah kata yang terdapat dalam SpellingCorrector ini.


**Returns:**
int - Jumlah kata yang terkandung dalam SpellingCorrector ini.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Mendapatkan koleksi kata yang saat ini terdapat dalam SpellingCorrector ini.


**Returns:**
java.lang.String[] - Koleksi kata.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Menambahkan koleksi kata yang ditentukan ke instance ini dari SpellingCorrector.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.Iterable<java.lang.String> | Koleksi kata untuk ditambahkan ke kamus. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Menambahkan koleksi kata yang ditentukan ke instance ini dari SpellingCorrector.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.String[] | Koleksi kata untuk ditambahkan ke kamus. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Menghapus semua kata dari objek SpellingCorrector.


