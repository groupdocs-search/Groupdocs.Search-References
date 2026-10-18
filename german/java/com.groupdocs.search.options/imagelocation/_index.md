---
title: "ImageLocation"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Gibt einen Bildspeicherort an."
type: docs
weight: 48
url: /de/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Gibt einen Bildspeicherort an.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Separate](#Separate) | Ein Bild in einer separaten Datei. |
|
|  | [Embedded](#Embedded) | Ein Bild, das in ein anderes Dokument eingebettet ist. |
|
|  | [ContainerItem](#ContainerItem) | Ein Bild, das ein Element in einer Containerdatei ist. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


Ein Bild in einer separaten Datei.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


Ein Bild, das in ein anderes Dokument eingebettet ist.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


Ein Bild, das ein Element in einer Containerdatei ist.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
