---
title: "DocumentImage"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili data gambar dokumen."
type: docs
weight: 16
url: /id/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Mewakili data gambar dokumen.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Mendapatkan nomor urut gambar dalam dokumen. |
|
|  | [getFields()](#getFields--) | Mendapatkan bidang yang diekstrak. |
|
|  | [getFrames()](#getFrames--) | Mendapatkan frame gambar. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Mendapatkan nomor urut gambar dalam dokumen.


**Returns:**
int - Nomor urut gambar dalam dokumen.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Mendapatkan bidang yang diekstrak.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Bidang yang diekstrak.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Mendapatkan frame gambar.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Frame gambar.

