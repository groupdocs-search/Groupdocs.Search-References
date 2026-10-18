---
title: "DocumentImage"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belge görüntü verisini temsil eder."
type: docs
weight: 16
url: /tr/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Belge görüntü verisini temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Belgedeki görüntünün sıra numarasını alır. |
|
|  | [getFields()](#getFields--) | Çıkarılan alanları alır. |
|
|  | [getFrames()](#getFrames--) | Görüntü karelerini alır. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Belgedeki görüntünün sıra numarasını alır.


**Returns:**
int - Belgedeki görüntünün sıra numarası.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Çıkarılan alanları alır.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Çıkarılan alanlar.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Görüntü karelerini alır.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Görüntü kareleri.

