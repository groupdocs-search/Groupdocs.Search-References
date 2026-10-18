---
title: "ImageLocation"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Specificeert een afbeeldingslocatie."
type: docs
weight: 48
url: /nl/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Specificeert een afbeeldingslocatie.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [Separate](#Separate) | Een afbeelding in een apart bestand. |
|
|  | [Embedded](#Embedded) | Een afbeelding ingebed in een ander document. |
|
|  | [ContainerItem](#ContainerItem) | Een afbeelding die een element is in een containerbestand. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


Een afbeelding in een apart bestand.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


Een afbeelding ingebed in een ander document.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


Een afbeelding die een element is in een containerbestand.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
