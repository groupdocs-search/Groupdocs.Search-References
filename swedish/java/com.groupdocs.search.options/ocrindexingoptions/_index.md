---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för OCR-behandling och indexering av igenkänd text."
type: docs
weight: 31
url: /sv/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Tillhandahåller alternativ för OCR-behandling och indexering av igenkänd text.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Hämtar ett värde som indikerar om text ska kännas igen i separata bildfiler. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Ställer in ett värde som indikerar om text ska kännas igen i separata bildfiler. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Hämtar ett värde som indikerar om text ska kännas igen i bilder som är objekt i en behållare (till exempel bilder i ett ZIP‑arkiv). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Ställer in ett värde som indikerar om text ska kännas igen i bilder som är objekt i en behållare (till exempel bilder i ett ZIP‑arkiv). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Hämtar ett värde som indikerar om text ska kännas igen i inbäddade bilder (till exempel bilder i ett DOCX‑dokument). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Ställer in ett värde som indikerar om text ska kännas igen i inbäddade bilder (till exempel bilder i ett DOCX‑dokument). |
|
|  | [getOcrConnector()](#getOcrConnector--) | Hämtar en OCR‑anslutning som används för OCR‑behandling. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Ställer in en OCR‑anslutning som används för OCR‑behandling. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Hämtar ett värde som indikerar om text ska kännas igen i separata bildfiler. Standardvärdet är false.


**Returns:**
boolean - Ett värde som indikerar om text ska kännas igen i separata bildfiler.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Ställer in ett värde som indikerar om text ska kännas igen i separata bildfiler. Standardvärdet är false.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om text ska kännas igen i separata bildfiler. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Hämtar ett värde som indikerar om text ska kännas igen i bilder som är objekt i en behållare (till exempel bilder i ett ZIP‑arkiv). Standardvärdet är false.


**Returns:**
boolean - Ett värde som indikerar om text ska kännas igen i bilder som är objekt i en behållare.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Ställer in ett värde som indikerar om text ska kännas igen i bilder som är objekt i en behållare (till exempel bilder i ett ZIP‑arkiv). Standardvärdet är false.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om text ska kännas igen i bilder som är objekt i en behållare. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Hämtar ett värde som indikerar om text ska kännas igen i inbäddade bilder (till exempel bilder i ett DOCX‑dokument). Standardvärdet är false.


**Returns:**
boolean - Ett värde som indikerar om text ska kännas igen i inbäddade bilder.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Ställer in ett värde som indikerar om text ska kännas igen i inbäddade bilder (till exempel bilder i ett DOCX‑dokument). Standardvärdet är false.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om text ska kännas igen i inbäddade bilder. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Hämtar en OCR‑anslutning som används för OCR‑behandling. Standardvärdet är null, vilket betyder att ingen OCR används.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Ställer in en OCR‑anslutning som används för OCR‑behandling. Standardvärdet är null, vilket betyder att ingen OCR används.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | En OCR‑anslutning som används för OCR‑behandling. |
|

