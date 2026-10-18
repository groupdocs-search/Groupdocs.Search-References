---
title: "TextStorageSettings"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili pengaturan penyimpanan teks."
type: docs
weight: 42
url: /id/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Mewakili pengaturan penyimpanan teks.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Menginisialisasi sebuah instance baru dari kelas  TextStorageSettings  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getCompression()](#getCompression--) | Mendapatkan kompresi penyimpanan teks. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Mengatur kompresi penyimpanan teks. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Menginisialisasi sebuah instance baru dari kelas  TextStorageSettings  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | Kompresi penyimpanan teks. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Mendapatkan kompresi penyimpanan teks. Nilai default adalah Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Mengatur kompresi penyimpanan teks. Nilai default adalah Compression.Normal.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | Kompresi penyimpanan teks. |
|

