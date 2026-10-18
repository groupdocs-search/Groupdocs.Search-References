---
title: "AliasDictionary"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mendefinisikan antarmuka kamus alias."
type: docs
weight: 14
url: /id/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Mendefinisikan antarmuka kamus alias.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCount()](#getCount--) | Mengambil jumlah alias yang terdapat dalam AliasDictionary. |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Menambahkan koleksi pasangan alias/pengganti yang ditentukan ke instance AliasDictionary ini. |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Menambahkan koleksi pasangan alias/pengganti yang ditentukan ke instance AliasDictionary ini. |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Menambahkan pasangan alias dan teks terkait yang ditentukan ke instance AliasDictionary ini. |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Menghapus alias yang ditentukan dari objek AliasDictionary. |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Menentukan apakah objek AliasDictionary berisi alias yang ditentukan. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Mengambil teks yang terkait dengan alias yang ditentukan. |
|
|  | [clear()](#clear--) | Menghapus semua alias dari objek AliasDictionary. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator yang mengiterasi koleksi. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Mengambil jumlah alias yang terdapat dalam AliasDictionary.


**Returns:**
int - Jumlah alias yang terdapat dalam AliasDictionary.

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Menambahkan koleksi pasangan alias/pengganti yang ditentukan ke instance AliasDictionary ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pasangan | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | Koleksi pasangan alias/pengganti untuk ditambahkan ke kamus. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Menambahkan koleksi pasangan alias/pengganti yang ditentukan ke instance AliasDictionary ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | Koleksi pasangan alias/pengganti untuk ditambahkan ke kamus. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Menambahkan pasangan alias dan teks terkait yang ditentukan ke instance AliasDictionary ini.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | alias | java.lang.String | Alias yang akan ditambahkan ke kamus. |
|
|  | teks | java.lang.String | Teks yang akan terkait dengan alias. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Menghapus alias yang ditentukan dari objek AliasDictionary.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | alias | java.lang.String | Alias yang akan dihapus. |
|

**Returns:**
boolean - Metode ini mengembalikan  true  jika alias berhasil ditemukan dan dihapus. Metode ini mengembalikan  false  jika alias tidak ditemukan dalam objek  AliasDictionary .

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Menentukan apakah objek AliasDictionary berisi alias yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | alias | java.lang.String | Alias yang akan dicari dalam objek  AliasDictionary . |
|

**Returns:**
boolean -  true  jika objek  AliasDictionary  berisi alias yang ditentukan; jika tidak,  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Mengambil teks yang terkait dengan alias yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | alias | java.lang.String | Alias yang akan dicari dalam objek  AliasDictionary . |
|

**Returns:**
java.lang.String - Teks yang terkait dengan alias yang ditentukan atau  null .

### clear() {#clear--}
```
public abstract void clear()
```


Menghapus semua alias dari objek AliasDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Mengembalikan iterator yang mengiterasi koleksi.


**Returns:**
java.util.Iterator<java.lang.String> - Iterator yang dapat digunakan untuk mengiterasi koleksi.

