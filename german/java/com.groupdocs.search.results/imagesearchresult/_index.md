---
title: "ImageSearchResult"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt das Ergebnis einer umgekehrten Bildsuche dar."
type: docs
weight: 17
url: /de/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Stellt das Ergebnis einer umgekehrten Bildsuche dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Gibt die Anzahl gefundener Bilder zurück. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Gibt das gefundene Bild nach Index zurück. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Gibt die Anzahl gefundener Bilder zurück.


**Returns:**
int - Die Anzahl gefundener Bilder.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Gibt das gefundene Bild nach Index zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Index | int | Der Index eines gefundenen Bildes. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

