---
title: "PasswordDictionary"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mendefinisikan antarmuka kamus kata sandi dokumen."
type: docs
weight: 20
url: /id/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Mendefinisikan antarmuka kamus kata sandi dokumen.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCount()](#getCount--) | Mendapatkan jumlah elemen yang terdapat dalam kamus. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Mendapatkan kata sandi untuk file. |
|
|  | [clear()](#clear--) | Menghapus semua kata sandi dari objek  PasswordDictionary  ini. |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Menentukan apakah kamus berisi kata sandi untuk dokumen yang ditentukan. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Menambahkan kata sandi untuk sebuah dokumen ke dalam kamus. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Menghapus kata sandi dokumen yang ditentukan dari kamus. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator yang mengiterasi koleksi. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Mendapatkan jumlah elemen yang terdapat dalam kamus.


**Returns:**
int - Jumlah elemen yang terdapat dalam kamus.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Mendapatkan kata sandi untuk file.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Path file. |
|

**Returns:**
java.lang.String - Kata sandi untuk file.

### clear() {#clear--}
```
public abstract void clear()
```


Menghapus semua kata sandi dari objek  PasswordDictionary  ini.


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Menentukan apakah kamus berisi kata sandi untuk dokumen yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Path file dokumen. |
|

**Returns:**
boolean -  true  jika kamus berisi kata sandi untuk dokumen; jika tidak,  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Menambahkan kata sandi untuk sebuah dokumen ke dalam kamus.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Path file dokumen. |
|
|  | kata sandi | java.lang.String | Kata sandi dokumen. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Menghapus kata sandi dokumen yang ditentukan dari kamus.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Path file dokumen. |
|

**Returns:**
boolean -  true  jika kata sandi berhasil dihapus; jika tidak,  false . Metode ini juga mengembalikan  false  jika  filePath  tidak ditemukan dalam kamus.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Mengembalikan iterator yang mengiterasi koleksi.


**Returns:**
java.util.Iterator<java.lang.String> - Iterator yang dapat digunakan untuk mengiterasi koleksi.

