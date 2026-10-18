---
title: "EnglishWordFormsProvider"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili penyedia bentuk kata bahasa Inggris."
type: docs
weight: 13
url: /id/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Mewakili penyedia bentuk kata bahasa Inggris.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Menginisialisasi instance baru dari |
EnglishWordFormsProvider
kelas.
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Mengambil bentuk kata untuk kata yang ditentukan. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Menginisialisasi instance baru dari
EnglishWordFormsProvider
kelas.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Mengambil bentuk kata untuk kata yang ditentukan.
Array hasil tidak berisi kata asli.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | kata | java.lang.String | Kata untuk menyarankan bentuk kata. |
|

**Returns:**
java.lang.String[] - Bentuk kata untuk kata yang ditentukan atau array kosong jika IWordFormsProvider tidak menyediakan bentuk kata untuk kata yang ditentukan.

