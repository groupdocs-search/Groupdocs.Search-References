---
title: "ImageSearchResult"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt het resultaat van een omgekeerde afbeeldingzoekopdracht voor."
type: docs
weight: 17
url: /nl/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Stelt het resultaat van een omgekeerde afbeeldingzoekopdracht voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Haalt het aantal gevonden afbeeldingen op. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Haalt de gevonden afbeelding op via index. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Haalt het aantal gevonden afbeeldingen op.


**Returns:**
int - Het aantal gevonden afbeeldingen.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Haalt de gevonden afbeelding op via index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | int | De index van een gevonden afbeelding. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

