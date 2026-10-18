---
title: "WordPattern"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili pola kata untuk digunakan dalam pencarian wildcard kata."
type: docs
weight: 34
url: /id/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Mewakili pola kata untuk digunakan dalam pencarian wildcard kata.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | Menginisialisasi instance baru dari kelas WordPattern. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Menambahkan string ke pola kata. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Menambahkan karakter ke pola kata. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Menambahkan wildcard satu karakter ke pola kata. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Menambahkan wildcard nol atau satu karakter ke pola kata. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Menambahkan wildcard nol atau lebih karakter ke pola kata. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Menambahkan wildcard satu atau lebih karakter ke pola kata. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Menambahkan wildcard ke pola kata. |
|
|  | [toString()](#toString--) | Mengembalikan sebuah  System.String  yang mewakili  WordPattern saat ini. |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Menginisialisasi instance baru dari kelas WordPattern.


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Menambahkan string ke pola kata.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | teks | java.lang.String | String yang akan ditambahkan. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Menambahkan karakter ke pola kata.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | karakter | char | Karakter yang akan ditambahkan. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Menambahkan wildcard satu karakter ke pola kata.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Menambahkan wildcard nol atau satu karakter ke pola kata.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Menambahkan wildcard nol atau lebih karakter ke pola kata.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Menambahkan wildcard satu atau lebih karakter ke pola kata.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Menambahkan wildcard ke pola kata.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | min | int | Jumlah minimum karakter. |
|
|  | max | int | Jumlah maksimum karakter. |
|

### toString() {#toString--}
```
public String toString()
```


Mengembalikan sebuah  System.String  yang mewakili  WordPattern saat ini.


**Returns:**
java.lang.String - Sebuah  System.String  yang mewakili  WordPattern saat ini.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
