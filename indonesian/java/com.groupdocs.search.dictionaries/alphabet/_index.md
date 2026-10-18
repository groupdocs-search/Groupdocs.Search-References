---
title: "Alphabet"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mendefinisikan antarmuka kamus karakter yang digunakan selama pengindeksan untuk mendeteksi tipe karakter."
type: docs
weight: 15
url: /id/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Mendefinisikan antarmuka kamus karakter yang digunakan selama pengindeksan untuk mendeteksi tipe karakter. Setiap karakter dapat diperlakukan sebagai pemisah, sebagai huruf, atau keduanya.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Mendapatkan tipe sebuah karakter. |
|
|  | [getCount()](#getCount--) | Mendapatkan jumlah karakter yang terdapat dalam Alphabet. |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Mengatur tipe untuk setiap karakter dari koleksi yang ditentukan dalam instance Alphabet ini. |
|
|  | [clear()](#clear--) | Mengatur tipe CharacterType.Separator untuk semua karakter dalam Alphabet ini. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator yang mengiterasi koleksi. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Mendapatkan tipe sebuah karakter.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | karakter | char | Karakter untuk mendapatkan tipe. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Mendapatkan jumlah karakter yang terdapat dalam Alphabet.


**Returns:**
int - Jumlah karakter dalam kamus.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Mengatur tipe untuk setiap karakter dari koleksi yang ditentukan dalam instance Alphabet ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | karakter | char[] | Koleksi karakter untuk mengatur tipe. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | Tipe karakter. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Mengatur tipe CharacterType.Separator untuk semua karakter dalam Alphabet ini.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Mengembalikan iterator yang mengiterasi koleksi.


**Returns:**
java.util.Iterator<java.lang.Character> - Iterator yang dapat digunakan untuk mengiterasi koleksi.

