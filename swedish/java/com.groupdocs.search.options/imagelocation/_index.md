---
title: "ImageLocation"
second_title: "GroupDocs.Search för Java API-referens"
description: "Specificerar en bildplats."
type: docs
weight: 48
url: /sv/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Specificerar en bildplats.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Separate](#Separate) | En bild i en separat fil. |
|
|  | [Embedded](#Embedded) | En bild inbäddad i ett annat dokument. |
|
|  | [ContainerItem](#ContainerItem) | En bild som är ett element i en containerfil. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


En bild i en separat fil.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


En bild inbäddad i ett annat dokument.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


En bild som är ett element i en containerfil.


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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
