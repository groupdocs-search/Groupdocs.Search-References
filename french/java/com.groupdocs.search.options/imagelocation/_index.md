---
title: "ImageLocation"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Spécifie un emplacement d'image."
type: docs
weight: 48
url: /fr/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Spécifie un emplacement d'image.

## Fields

| Field | Description |
| --- | --- |
|  | [Separate](#Separate) | Une image dans un fichier séparé. |
|
|  | [Embedded](#Embedded) | Une image incorporée dans un autre document. |
|
|  | [ContainerItem](#ContainerItem) | Une image qui est un élément dans un fichier conteneur. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


Une image dans un fichier séparé.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


Une image incorporée dans un autre document.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


Une image qui est un élément dans un fichier conteneur.


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
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
