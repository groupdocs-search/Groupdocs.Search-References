---
title: "FragmentContainer"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili wadah untuk fragmen teks dengan istilah yang ditemukan disorot dari satu bidang dokumen."
type: docs
weight: 22
url: /id/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Mewakili wadah untuk fragmen teks dengan istilah yang ditemukan disorot dari satu bidang dokumen.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Mendapatkan nama bidang dokumen. |
|
|  | [getCount()](#getCount--) | Mendapatkan jumlah fragmen teks yang terkandung. |
|
|  | [getFragments()](#getFragments--) | Mendapatkan array fragmen teks yang terkandung. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Mendapatkan nama bidang dokumen.


**Returns:**
java.lang.String - Nama bidang dokumen.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Mendapatkan jumlah fragmen teks yang terkandung.


**Returns:**
int - Jumlah fragmen teks yang terkandung.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Mendapatkan array fragmen teks yang terkandung.


**Returns:**
java.lang.String[] - Array fragmen teks yang terkandung.

