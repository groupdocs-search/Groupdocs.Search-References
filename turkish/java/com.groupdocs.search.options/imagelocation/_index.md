---
title: "ImageLocation"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir görüntü konumu belirtir."
type: docs
weight: 48
url: /tr/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Bir görüntü konumu belirtir.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [Separate](#Separate) | Ayrı bir dosyada bir görüntü. |
|
|  | [Embedded](#Embedded) | Başka bir belgeye gömülmüş bir görüntü. |
|
|  | [ContainerItem](#ContainerItem) | Bir kapsayıcı dosyasında bir öğe olan görüntü. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


Ayrı bir dosyada bir görüntü.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


Başka bir belgeye gömülmüş bir görüntü.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


Bir kapsayıcı dosyasında bir öğe olan görüntü.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
