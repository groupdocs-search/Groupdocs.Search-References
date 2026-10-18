---
title: "ImageLocation"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Especifica una ubicación de imagen."
type: docs
weight: 48
url: /es/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Especifica una ubicación de imagen.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Separate](#Separate) | Una imagen en un archivo separado. |
|
|  | [Embedded](#Embedded) | Una imagen incrustada en otro documento. |
|
|  | [ContainerItem](#ContainerItem) | Una imagen que es un elemento en un archivo contenedor. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


Una imagen en un archivo separado.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


Una imagen incrustada en otro documento.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


Una imagen que es un elemento en un archivo contenedor.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
