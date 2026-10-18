---
title: "CharacterReplacementDictionary"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mendefinisikan antarmuka kamus pengganti karakter yang digunakan selama proses pengindeksan."
type: docs
weight: 16
url: /id/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Mendefinisikan antarmuka kamus penggantian karakter yang digunakan selama proses pengindeksan. Penggantian karakter dapat digunakan, misalnya, untuk menghapus aksen dari karakter beraksen atau untuk membuat indeks tidak sensitif huruf.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCount()](#getCount--) | Mendapatkan jumlah karakter yang terdapat dalam  CharacterReplacementDictionary  ini. |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Menambahkan koleksi penggantian karakter yang ditentukan ke instance ini dari  CharacterReplacementDictionary . |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Menambahkan koleksi penggantian karakter yang ditentukan ke instance ini dari  CharacterReplacementDictionary . |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Menghapus koleksi penggantian karakter yang ditentukan dari instance ini dari CharacterReplacementDictionary. |
|
|  | [contains(char character)](#contains-char-) | Menentukan apakah objek CharacterReplacementDictionary berisi penggantian untuk karakter yang ditentukan. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Mendapatkan penggantian untuk karakter yang ditentukan. |
|
|  | [clear()](#clear--) | Menghapus semua penggantian karakter dari objek CharacterReplacementDictionary. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator yang mengiterasi koleksi. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Mendapatkan jumlah karakter yang terdapat dalam  CharacterReplacementDictionary  ini.


**Returns:**
int - Jumlah karakter dalam kamus.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Menambahkan koleksi penggantian karakter yang ditentukan ke instance ini dari  CharacterReplacementDictionary .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | Koleksi penggantian karakter untuk ditambahkan ke kamus. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Menambahkan koleksi penggantian karakter yang ditentukan ke instance ini dari  CharacterReplacementDictionary .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | Koleksi penggantian karakter untuk ditambahkan ke kamus. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Menghapus koleksi penggantian karakter yang ditentukan dari instance ini dari CharacterReplacementDictionary.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | karakter | char[] | Koleksi karakter untuk dihapus. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Menentukan apakah objek CharacterReplacementDictionary berisi penggantian untuk karakter yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | karakter | char | Karakter yang akan dicari dalam objek CharacterReplacementDictionary. |
|

**Returns:**
boolean - true jika objek CharacterReplacementDictionary berisi karakter yang ditentukan; jika tidak, false.

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Mendapatkan penggantian untuk karakter yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | karakter | char | Karakter untuk mendapatkan penggantian. |
|

**Returns:**
char - Pengganti untuk karakter yang ditentukan.

### clear() {#clear--}
```
public abstract void clear()
```


Menghapus semua penggantian karakter dari objek CharacterReplacementDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Mengembalikan iterator yang mengiterasi koleksi.


**Returns:**
java.util.Iterator<java.lang.Character> - Iterator yang dapat digunakan untuk mengiterasi koleksi.

