---
title: "AttributeChangeBatch"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili wadah untuk perubahan atribut."
type: docs
weight: 10
url: /id/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Mewakili wadah untuk perubahan atribut.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | Menginisialisasi instance baru dari kelas AttributeChangeBatch. |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | Menginisialisasi instance baru dari kelas AttributeChangeBatch. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Menambahkan atribut yang ditentukan ke dokumen terindeks yang ditentukan. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Menambahkan atribut yang ditentukan ke dokumen-dokumen terindeks yang ditentukan. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Menambahkan atribut yang ditentukan ke semua dokumen dalam indeks. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Menghapus atribut yang ditentukan dari dokumen terindeks yang ditentukan. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Menghapus atribut yang ditentukan dari dokumen-dokumen terindeks yang ditentukan. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Menghapus semua atribut dari dokumen terindeks yang ditentukan. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Menghapus semua atribut dari dokumen-dokumen terindeks yang ditentukan. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Menghapus atribut yang ditentukan dari semua dokumen dalam indeks. |
|
|  | [clear()](#clear--) | Menghapus semua atribut dari semua dokumen dalam indeks. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


Menginisialisasi instance baru dari kelas AttributeChangeBatch.


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


Menginisialisasi instance baru dari kelas AttributeChangeBatch.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | java.lang.Object | Data yang diserialkan. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Menambahkan atribut yang ditentukan ke dokumen terindeks yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | path | java.lang.String | Jalur dokumen. |
|
|  | atribut | java.lang.String[] | Atribut yang akan ditambahkan. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Menambahkan atribut yang ditentukan ke dokumen-dokumen terindeks yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | jalur | java.lang.String[] | Jalur dokumen. |
|
|  | atribut | java.lang.String[] | Atribut yang akan ditambahkan. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Menambahkan atribut yang ditentukan ke semua dokumen dalam indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | atribut | java.lang.String[] | Atribut yang akan ditambahkan. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Menghapus atribut yang ditentukan dari dokumen terindeks yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | path | java.lang.String | Jalur dokumen. |
|
|  | atribut | java.lang.String[] | Atribut yang akan dihapus. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Menghapus atribut yang ditentukan dari dokumen-dokumen terindeks yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | jalur | java.lang.String[] | Jalur dokumen. |
|
|  | atribut | java.lang.String[] | Atribut yang akan dihapus. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Menghapus semua atribut dari dokumen terindeks yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | path | java.lang.String | Jalur dokumen. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Menghapus semua atribut dari dokumen-dokumen terindeks yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | jalur | java.lang.String[] | Jalur dokumen. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


Menghapus atribut yang ditentukan dari semua dokumen dalam indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | atribut | java.lang.String[] | Atribut yang akan dihapus. |
|

### clear() {#clear--}
```
public void clear()
```


Menghapus semua atribut dari semua dokumen dalam indeks.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
