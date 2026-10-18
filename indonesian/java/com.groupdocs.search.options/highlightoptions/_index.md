---
title: "HighlightOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk menyorot istilah yang ditemukan."
type: docs
weight: 22
url: /id/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Menyediakan opsi untuk menyorot istilah yang ditemukan.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Menginisialisasi instance baru dari kelas HighlightOptions. |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Menginisialisasi instance baru dari kelas TextOptions. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Mendapatkan jumlah maksimum kata dalam cuplikan teks sebelum kata yang disorot. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Mengatur jumlah maksimum kata dalam cuplikan teks sebelum kata yang disorot. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Mendapatkan jumlah maksimum kata dalam cuplikan teks setelah kata yang disorot. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Mengatur jumlah maksimum kata dalam cuplikan teks setelah kata yang disorot. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Mendapatkan jumlah maksimum kata dalam cuplikan teks. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Mengatur jumlah maksimum kata dalam cuplikan teks. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Mendapatkan nilai yang menunjukkan apakah gaya inline digunakan untuk menyorot kemunculan. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Mengatur nilai yang menunjukkan apakah gaya inline digunakan untuk menyorot kemunculan. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Mendapatkan warna yang digunakan untuk menyorot kemunculan. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Mengatur warna yang digunakan untuk menyorot kemunculan. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Mendapatkan tag awal penyorotan kata yang ditemukan. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Mengatur tag awal penyorotan kata yang ditemukan. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Mendapatkan tag akhir penyorotan kata yang ditemukan. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Mengatur tag akhir penyorotan kata yang ditemukan. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Menginisialisasi instance baru dari kelas HighlightOptions.


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Menginisialisasi instance baru dari kelas TextOptions.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | data | java.lang.Object | Data yang diserialkan. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Mendapatkan jumlah maksimum kata dalam cuplikan teks sebelum kata yang disorot. Nilai harus berada dalam rentang 0 hingga 10000. Nilai default adalah 7.


**Returns:**
int - Jumlah maksimum kata dalam cuplikan teks sebelum kata yang disorot.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Mengatur jumlah maksimum kata dalam cuplikan teks sebelum kata yang disorot. Nilai harus berada dalam rentang 0 hingga 10000. Nilai default adalah 7.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum kata dalam cuplikan teks sebelum kata yang disorot. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Mendapatkan jumlah maksimum kata dalam cuplikan teks setelah kata yang disorot. Nilai harus berada dalam rentang 0 hingga 10000. Nilai default adalah 7.


**Returns:**
int - Jumlah maksimum kata dalam cuplikan teks setelah kata yang disorot.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Mengatur jumlah maksimum kata dalam cuplikan teks setelah kata yang disorot. Nilai harus berada dalam rentang 0 hingga 10000. Nilai default adalah 7.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum kata dalam cuplikan teks setelah kata yang disorot. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Mendapatkan jumlah maksimum kata dalam cuplikan teks. Nilai harus berada dalam rentang 0 hingga 10000. Nilai default adalah 21.


**Returns:**
int - Jumlah maksimum kata dalam cuplikan teks.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Mengatur jumlah maksimum kata dalam cuplikan teks. Nilai harus berada dalam rentang 0 hingga 10000. Nilai default adalah 21.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum kata dalam cuplikan teks. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Mendapatkan nilai yang menunjukkan apakah gaya inline digunakan untuk menyorot kemunculan. Nilai default adalah true.


**Returns:**
boolean - Nilai yang menunjukkan apakah gaya inline digunakan untuk menyorot kemunculan.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Mengatur nilai yang menunjukkan apakah gaya inline digunakan untuk menyorot kemunculan. Nilai default adalah true.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah gaya inline digunakan untuk menyorot kemunculan. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Mendapatkan warna yang digunakan untuk menyorot kemunculan. Nilai default adalah #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Mengatur warna yang digunakan untuk menyorot kemunculan. Nilai default adalah #FFD800.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | Sebuah warna yang digunakan untuk menyorot kemunculan. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Mendapatkan tag pembuka penyorotan kata yang ditemukan. Tag ini hanya digunakan saat menyorot dalam teks biasa. Nilai default adalah string kosong.


**Returns:**
java.lang.String - Tag pembuka penyorotan kata yang ditemukan.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Mengatur tag pembuka penyorotan kata yang ditemukan. Tag ini hanya digunakan saat menyorot dalam teks biasa. Nilai default adalah string kosong.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Tag pembuka penyorotan kata yang ditemukan. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Mendapatkan tag penutup penyorotan kata yang ditemukan. Tag ini hanya digunakan saat menyorot dalam teks biasa. Nilai default adalah string kosong.


**Returns:**
java.lang.String - Tag penutup penyorotan kata yang ditemukan.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Mengatur tag penutup penyorotan kata yang ditemukan. Tag ini hanya digunakan saat menyorot dalam teks biasa. Nilai default adalah string kosong.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Tag penutup penyorotan kata yang ditemukan. |
|

