---
title: "ImageSearchResult"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar resultatet av en omvänd bildsökning."
type: docs
weight: 17
url: /sv/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Representerar resultatet av en omvänd bildsökning.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Hämtar antalet hittade bilder. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Hämtar den hittade bilden efter index. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Hämtar antalet hittade bilder.


**Returns:**
int - Antalet hittade bilder.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Hämtar den hittade bilden efter index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Indexet för en hittad bild. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

