---
title: "SearchImage"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en bild att söka efter."
type: docs
weight: 29
url: /sv/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Representerar en bild att söka efter.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Skapar en bild från en fil för sökning. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Skapar en bild från en fil för sökning. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Skapar en bild från en ström för sökning. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Skapar en bild från en ström för sökning. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Skapar en bild från en fil för sökning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till bildfilen. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Skapar en bild från en fil för sökning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökvägen till bildfilen. |
|
|  | imageIndex | int | Bildens index i flersidiga bilder. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Skapar en bild från en ström för sökning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ström | java.io.InputStream | Bildströmmen. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Skapar en bild från en ström för sökning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ström | java.io.InputStream | Bildströmmen. |
|
|  | imageIndex | int | Bildens index i flersidiga bilder. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

