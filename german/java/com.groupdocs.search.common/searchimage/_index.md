---
title: "SearchImage"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein zu suchendes Bild dar."
type: docs
weight: 29
url: /de/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Stellt ein zu suchendes Bild dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Erstellt ein Bild aus einer Datei zum Durchsuchen. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Erstellt ein Bild aus einer Datei zum Durchsuchen. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Erstellt ein Bild aus einem Stream zum Durchsuchen. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Erstellt ein Bild aus einem Stream zum Durchsuchen. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Erstellt ein Bild aus einer Datei zum Durchsuchen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Bilddatei. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Erstellt ein Bild aus einer Datei zum Durchsuchen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad zur Bilddatei. |
|
|  | imageIndex | int | Der Bildindex in mehrseitigen Bildern. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Erstellt ein Bild aus einem Stream zum Durchsuchen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | stream | java.io.InputStream | Der Bild-Stream. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Erstellt ein Bild aus einem Stream zum Durchsuchen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | stream | java.io.InputStream | Der Bild-Stream. |
|
|  | imageIndex | int | Der Bildindex in mehrseitigen Bildern. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

