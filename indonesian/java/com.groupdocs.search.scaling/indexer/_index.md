---
title: "Indexer"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili layanan yang mengelola distribusi dokumen terindeks di seluruh shard jaringan pencarian."
type: docs
weight: 10
url: /id/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Mewakili layanan yang mengelola distribusi dokumen terindeks di seluruh shard jaringan pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Melakukan operasi pengindeksan. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Melakukan operasi pengindeksan. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Menghapus dokumen yang diindeks. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Meminimalkan jumlah segmen indeks dengan menggabungkannya satu dengan yang lain. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Menyinkronkan daftar dokumen yang diindeks dengan yang ada di shard. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Menerapkan batch perubahan atribut yang ditentukan ke dokumen yang diindeks tanpa melakukan pengindeksan ulang. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Mendapatkan semua atribut yang terkait dengan dokumen yang diindeks yang ditentukan. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Mendapatkan kamus dari shard yang ditentukan. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Mendapatkan kamus alfabet. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Mendapatkan kamus alias. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Mendapatkan kamus penggantian karakter. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Mendapatkan kamus sinonim. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Mendapatkan kamus homofon. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Mendapatkan kamus korektor ejaan. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Mendapatkan kamus kata berhenti. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Mendapatkan kamus kata sandi. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Menetapkan kamus pada shard yang ditentukan. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Menetapkan kamus pada semua shard. |
|
|  | [deleteAllData()](#deleteAllData--) | Menghapus semua data terindeks dari semua shard jaringan pencarian. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Melakukan operasi pengindeksan. Hanya pengindeksan dari aliran dan struktur yang didukung.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Dokumen dari sistem file, aliran, atau struktur. |
|
|  | kata sandi | java.lang.String[] | Kata sandi dokumen. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Opsi penambahan. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Melakukan operasi pengindeksan. Menambahkan data yang diekstrak ke jaringan pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Data yang diekstrak. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Opsi pengindeksan. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Menghapus dokumen yang diindeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | Kunci dokumen yang ditambahkan dari aliran atau struktur. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | Opsi penghapusan. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Meminimalkan jumlah segmen indeks dengan menggabungkannya satu sama lain. Operasi ini meningkatkan kinerja pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | Opsi optimasi. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Menyinkronkan daftar dokumen terindeks dengan yang ada pada shard. Operasi ini memperbaiki masalah pengindeksan dan penghapusan dokumen yang disebabkan oleh masalah komunikasi dengan node jaringan pencarian.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | Opsi sinkronisasi. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Menerapkan batch perubahan atribut yang ditentukan ke dokumen yang diindeks tanpa melakukan pengindeksan ulang.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Batch perubahan atribut. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | Opsi mengubah atribut. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Mendapatkan semua atribut yang terkait dengan dokumen yang diindeks yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentKey | java.lang.String | Kunci dokumen. |
|

**Returns:**
java.lang.String[] - Atribut yang terkait dengan dokumen terindeks yang ditentukan.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Mendapatkan kamus dari shard yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | Jenis kamus. |
|
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Mendapatkan kamus alfabet.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Mendapatkan kamus alias.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Mendapatkan kamus penggantian karakter.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Mendapatkan kamus sinonim.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Mendapatkan kamus homofon.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Mendapatkan kamus korektor ejaan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Mendapatkan kamus kata berhenti.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Mendapatkan kamus kata sandi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Menetapkan kamus pada shard yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Kamus. |
|
|  | shardIndex | int | Indeks shard. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Menetapkan kamus pada semua shard.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Kamus. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Menghapus semua data terindeks dari semua shard jaringan pencarian.


