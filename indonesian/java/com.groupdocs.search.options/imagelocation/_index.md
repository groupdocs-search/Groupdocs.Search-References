---
title: "ImageLocation"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menentukan lokasi gambar."
type: docs
weight: 48
url: /id/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Menentukan lokasi gambar.

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [Separate](#Separate) | Sebuah gambar dalam file terpisah. |
|
|  | [Embedded](#Embedded) | Sebuah gambar yang disematkan dalam dokumen lain. |
|
|  | [ContainerItem](#ContainerItem) | Sebuah gambar yang merupakan elemen dalam file kontainer. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


Sebuah gambar dalam file terpisah.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


Sebuah gambar yang disematkan dalam dokumen lain.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


Sebuah gambar yang merupakan elemen dalam file kontainer.


### values() {#values--}
```
public static ImageLocation[] values()
```




**Returns:**
com.groupdocs.search.options.ImageLocation[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ImageLocation valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
