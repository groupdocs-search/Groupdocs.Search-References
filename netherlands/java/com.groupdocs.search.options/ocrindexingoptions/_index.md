---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor OCR-verwerking en het indexeren van herkende tekst."
type: docs
weight: 31
url: /nl/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Biedt opties voor OCR-verwerking en het indexeren van herkende tekst.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Haalt een waarde op die aangeeft of tekst moet worden herkend in afzonderlijke afbeeldingsbestanden. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Stelt een waarde in die aangeeft of tekst moet worden herkend in afzonderlijke afbeeldingsbestanden. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Haalt een waarde op die aangeeft of tekst moet worden herkend in afbeeldingen die items zijn in een container (bijvoorbeeld afbeeldingen in een ZIP-archief). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Stelt een waarde in die aangeeft of tekst moet worden herkend in afbeeldingen die items zijn in een container (bijvoorbeeld afbeeldingen in een ZIP-archief). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Haalt een waarde op die aangeeft of tekst moet worden herkend in ingesloten afbeeldingen (bijvoorbeeld afbeeldingen in een DOCX-document). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Stelt een waarde in die aangeeft of tekst moet worden herkend in ingesloten afbeeldingen (bijvoorbeeld afbeeldingen in een DOCX-document). |
|
|  | [getOcrConnector()](#getOcrConnector--) | Haalt een OCR-connector op die wordt gebruikt voor OCR-verwerking. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Stelt een OCR-connector in die wordt gebruikt voor OCR-verwerking. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Haalt een waarde op die aangeeft of tekst moet worden herkend in afzonderlijke afbeeldingsbestanden. De standaardwaarde is false.


**Returns:**
boolean - Een waarde die aangeeft of tekst moet worden herkend in afzonderlijke afbeeldingsbestanden.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Stelt een waarde in die aangeeft of tekst moet worden herkend in afzonderlijke afbeeldingsbestanden. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of tekst moet worden herkend in afzonderlijke afbeeldingsbestanden. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Haalt een waarde op die aangeeft of tekst moet worden herkend in afbeeldingen die items zijn in een container (bijvoorbeeld afbeeldingen in een ZIP-archief). De standaardwaarde is false.


**Returns:**
boolean - Een waarde die aangeeft of tekst moet worden herkend in afbeeldingen die items zijn in een container.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Stelt een waarde in die aangeeft of tekst moet worden herkend in afbeeldingen die items zijn in een container (bijvoorbeeld afbeeldingen in een ZIP-archief). De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of tekst moet worden herkend in afbeeldingen die items zijn in een container. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Haalt een waarde op die aangeeft of tekst moet worden herkend in ingesloten afbeeldingen (bijvoorbeeld afbeeldingen in een DOCX-document). De standaardwaarde is false.


**Returns:**
boolean - Een waarde die aangeeft of tekst moet worden herkend in ingesloten afbeeldingen.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Stelt een waarde in die aangeeft of tekst moet worden herkend in ingesloten afbeeldingen (bijvoorbeeld afbeeldingen in een DOCX-document). De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of tekst moet worden herkend in ingesloten afbeeldingen. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Haalt een OCR-connector op die wordt gebruikt voor OCR-verwerking. De standaardwaarde is null, wat betekent dat er geen OCR wordt gebruikt.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Stelt een OCR-connector in die wordt gebruikt voor OCR-verwerking. De standaardwaarde is null, wat betekent dat er geen OCR wordt gebruikt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Een OCR-connector die wordt gebruikt voor OCR-verwerking. |
|

