---
title: "SearchImage"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een afbeelding voor om te zoeken."
type: docs
weight: 29
url: /nl/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Stelt een afbeelding voor om te zoeken.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Maakt een afbeelding van een bestand om te doorzoeken. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Maakt een afbeelding van een bestand om te doorzoeken. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Maakt een afbeelding van een stream om te doorzoeken. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Maakt een afbeelding van een stream om te doorzoeken. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Maakt een afbeelding van een bestand om te doorzoeken.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het afbeeldingsbestand. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Maakt een afbeelding van een bestand om te doorzoeken.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad naar het afbeeldingsbestand. |
|
|  | imageIndex | int | De afbeeldingsindex in meerpagina-afbeeldingen. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Maakt een afbeelding van een stream om te doorzoeken.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | stream | java.io.InputStream | De afbeeldingsstream. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Maakt een afbeelding van een stream om te doorzoeken.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | stream | java.io.InputStream | De afbeeldingsstream. |
|
|  | imageIndex | int | De afbeeldingsindex in meerpagina-afbeeldingen. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

