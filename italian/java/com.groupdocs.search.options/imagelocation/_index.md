---
title: "ImageLocation"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Specifica una posizione dell'immagine."
type: docs
weight: 48
url: /it/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Specifica una posizione dell'immagine.

## Fields

| Field | Descrizione |
| --- | --- |
|  | [Separate](#Separate) | Un'immagine in un file separato. |
|
|  | [Embedded](#Embedded) | Un'immagine incorporata in un altro documento. |
|
|  | [ContainerItem](#ContainerItem) | Un'immagine che è un elemento in un file contenitore. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


Un'immagine in un file separato.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


Un'immagine incorporata in un altro documento.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


Un'immagine che è un elemento in un file contenitore.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
