---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Optionen für die OCR-Verarbeitung und das Indexieren erkannter Texte bereit."
type: docs
weight: 31
url: /de/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Stellt Optionen für die OCR-Verarbeitung und das Indexieren erkannter Texte bereit.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Ermittelt einen Wert, der angibt, ob Text in separaten Bilddateien erkannt werden soll. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Legt einen Wert fest, der angibt, ob Text in separaten Bilddateien erkannt werden soll. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Ermittelt einen Wert, der angibt, ob Text in Bildern erkannt werden soll, die Elemente in einem Container sind (z. B. Bilder in einem ZIP-Archiv). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Legt einen Wert fest, der angibt, ob Text in Bildern erkannt werden soll, die Elemente in einem Container sind (z. B. Bilder in einem ZIP-Archiv). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Ermittelt einen Wert, der angibt, ob Text in eingebetteten Bildern erkannt werden soll (z. B. Bilder in einem DOCX-Dokument). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Legt einen Wert fest, der angibt, ob Text in eingebetteten Bildern erkannt werden soll (z. B. Bilder in einem DOCX-Dokument). |
|
|  | [getOcrConnector()](#getOcrConnector--) | Ermittelt einen OCR‑Connector, der für die OCR‑Verarbeitung verwendet wird. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Legt einen OCR‑Connector fest, der für die OCR‑Verarbeitung verwendet wird. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Ermittelt einen Wert, der angibt, ob Text in separaten Bilddateien erkannt werden soll. Der Standardwert ist  false .


**Returns:**
boolean - Ein Wert, der angibt, ob Text in separaten Bilddateien erkannt werden soll.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Legt einen Wert fest, der angibt, ob Text in separaten Bilddateien erkannt werden soll. Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob Text in separaten Bilddateien erkannt werden soll. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Ermittelt einen Wert, der angibt, ob Text in Bildern erkannt werden soll, die Elemente in einem Container sind (z. B. Bilder in einem ZIP-Archiv). Der Standardwert ist  false .


**Returns:**
boolean - Ein Wert, der angibt, ob Text in Bildern erkannt werden soll, die Elemente in einem Container sind.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Legt einen Wert fest, der angibt, ob Text in Bildern erkannt werden soll, die Elemente in einem Container sind (z. B. Bilder in einem ZIP-Archiv). Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob Text in Bildern erkannt werden soll, die Elemente in einem Container sind. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Ermittelt einen Wert, der angibt, ob Text in eingebetteten Bildern erkannt werden soll (z. B. Bilder in einem DOCX-Dokument). Der Standardwert ist  false .


**Returns:**
boolean - Ein Wert, der angibt, ob Text in eingebetteten Bildern erkannt werden soll.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Legt einen Wert fest, der angibt, ob Text in eingebetteten Bildern erkannt werden soll (z. B. Bilder in einem DOCX-Dokument). Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob Text in eingebetteten Bildern erkannt werden soll. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Ermittelt einen OCR‑Connector, der für die OCR‑Verarbeitung verwendet wird. Der Standardwert ist  null , was bedeutet, dass keine OCR verwendet wird.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Legt einen OCR‑Connector fest, der für die OCR‑Verarbeitung verwendet wird. Der Standardwert ist  null , was bedeutet, dass keine OCR verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Ein OCR‑Connector, der für die OCR‑Verarbeitung verwendet wird. |
|

