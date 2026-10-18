---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för bildindexering för omvänd bildsökning."
type: docs
weight: 23
url: /sv/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Tillhandahåller alternativ för bildindexering för omvänd bildsökning.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Hämtar ett värde som indikerar om separata bildfiler ska indexeras. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Ställer in ett värde som indikerar om separata bildfiler ska indexeras. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Hämtar ett värde som indikerar om bilder som är objekt i en behållare ska indexeras (till exempel bilder i ett ZIP‑arkiv). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Ställer in ett värde som indikerar om bilder som är objekt i en behållare ska indexeras (till exempel bilder i ett ZIP‑arkiv). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Hämtar ett värde som indikerar om inbäddade bilder ska indexeras (till exempel bilder i ett DOCX‑dokument). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Ställer in ett värde som indikerar om inbäddade bilder ska indexeras (till exempel bilder i ett DOCX‑dokument). |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Hämtar ett värde som indikerar om separata bildfiler ska indexeras. Standardvärdet är  false .


**Returns:**
boolean - Ett värde som indikerar om separata bildfiler ska indexeras.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Ställer in ett värde som indikerar om separata bildfiler ska indexeras. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om separata bildfiler ska indexeras. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Hämtar ett värde som indikerar om bilder som är objekt i en behållare ska indexeras (till exempel bilder i ett ZIP‑arkiv). Standardvärdet är  false .


**Returns:**
boolean - Ett värde som indikerar om bilder som är objekt i en behållare ska indexeras.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Ställer in ett värde som indikerar om bilder som är objekt i en behållare (till exempel bilder i ett ZIP‑arkiv) ska indexeras. Standardvärdet är false.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om bilder som är objekt i en behållare ska indexeras. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Hämtar ett värde som indikerar om inbäddade bilder (till exempel bilder i ett DOCX‑dokument) ska indexeras. Standardvärdet är false.


**Returns:**
boolean - Ett värde som indikerar om inbäddade bilder ska indexeras.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Ställer in ett värde som indikerar om inbäddade bilder (till exempel bilder i ett DOCX‑dokument) ska indexeras. Standardvärdet är false.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om inbäddade bilder ska indexeras. |
|

