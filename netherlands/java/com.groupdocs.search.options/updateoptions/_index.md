---
title: "UpdateOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor de updatebewerking."
type: docs
weight: 43
url: /nl/java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

Biedt opties voor de updatebewerking.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)
* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [UpdateOptions()](#UpdateOptions--) | Initialiseert een nieuw exemplaar van de  UpdateOptions  klasse. |
|
|  | [UpdateOptions(Object data)](#UpdateOptions-java.lang.Object-) | Initialiseert een nieuw exemplaar van de  UpdateOptions  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getThreads()](#getThreads--) | Haalt het aantal threads op dat wordt gebruikt voor indexeren. |
|
|  | [setThreads(int value)](#setThreads-int-) | Stelt het aantal threads in dat wordt gebruikt voor indexeren. |
|
|  | [isAsync()](#isAsync--) | Haalt de vlag op van asynchrone uitvoering van de bewerking. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Stelt de vlag in van asynchrone uitvoering van de bewerking. |
|
|  | [getCancellation()](#getCancellation--) | Haalt het annuleringsobject van de bewerking op. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Stelt het annuleringsobject van de bewerking in. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Haalt een waarde op die aangeeft of de codering automatisch moet worden gedetecteerd of niet. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Stelt een waarde in die aangeeft of de codering automatisch moet worden gedetecteerd of niet. |
|
|  | [getEncoding()](#getEncoding--) | Haalt de codering op die wordt gebruikt om tekst uit tekstdocumenten te extraheren. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Stelt de codering in die wordt gebruikt om tekst uit tekstdocumenten te extraheren. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Haalt een waarde op die aangeeft of de ruwe modus wordt gebruikt voor tekstelextractie indien mogelijk. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Stelt een waarde in die aangeeft of de ruwe modus wordt gebruikt voor tekstelextractie indien mogelijk. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Haalt de opties op voor het indexeren van metagegevensvelden. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Haalt de opties op voor OCR-verwerking en het indexeren van herkende tekst. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Haalt de afbeeldingsindexeringsopties op voor omgekeerd zoeken naar afbeeldingen. |
|
| [getCore()](#getCore--) |  |
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


Initialiseert een nieuw exemplaar van de  UpdateOptions  klasse.


### UpdateOptions(Object data) {#UpdateOptions-java.lang.Object-}
```
public UpdateOptions(Object data)
```


Initialiseert een nieuw exemplaar van de  UpdateOptions  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | gegevens | java.lang.Object | De geserialiseerde gegevens. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Haalt het aantal threads op dat wordt gebruikt voor indexeren. De standaardwaarde is 1.


**Returns:**
int - Het aantal threads dat wordt gebruikt voor indexeren.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Stelt het aantal threads in dat wordt gebruikt voor indexeren. De standaardwaarde is 1.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het aantal threads dat wordt gebruikt voor indexeren. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Haalt de vlag op voor asynchrone uitvoering van de bewerking. De standaardwaarde is false.


**Returns:**
boolean - De vlag voor asynchrone uitvoering van de bewerking.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Stelt de vlag in voor asynchrone uitvoering van de bewerking. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlag voor asynchrone uitvoering van de bewerking. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Haalt het annuleringsobject van de bewerking op. De standaardwaarde is null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Stelt het annuleringsobject van de bewerking in. De standaardwaarde is null.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Het annuleringsobject van de bewerking. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Haalt een waarde op die aangeeft of de codering automatisch moet worden gedetecteerd of niet. De standaardwaarde is false.


**Returns:**
boolean - Een waarde die aangeeft of de codering automatisch moet worden gedetecteerd of niet.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Stelt een waarde in die aangeeft of de codering automatisch moet worden gedetecteerd of niet. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of de codering automatisch moet worden gedetecteerd of niet. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Haalt de codering op die wordt gebruikt om tekst uit tekstdocumenten te extraheren. De standaardwaarde is null, wat betekent dat de standaardcodering UTF-8 wordt gebruikt. Als AutoDetectEncoding true is, wordt deze waarde als standaardcodering gebruikt.


**Returns:**
java.lang.String - De codering die wordt gebruikt om tekst uit tekstdocumenten te extraheren.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Stelt de codering in die wordt gebruikt om tekst uit tekstdocumenten te extraheren. De standaardwaarde is null, wat betekent dat de standaardcodering UTF-8 wordt gebruikt. Als AutoDetectEncoding true is, wordt deze waarde als standaardcodering gebruikt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De codering die wordt gebruikt om tekst uit tekstdocumenten te extraheren. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Haalt een waarde op die aangeeft of de ruwe modus wordt gebruikt voor teksteextractie indien mogelijk. De standaardwaarde is  true . De ruwe modus kan de indexeringssnelheid aanzienlijk verhogen, maar de normale modus verbetert de opmaak van de geëxtraheerde tekst.


**Returns:**
boolean - Een waarde die aangeeft of de ruwe modus wordt gebruikt voor teksteextractie indien mogelijk.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Stelt een waarde in die aangeeft of de ruwe modus wordt gebruikt voor teksteextractie indien mogelijk. De standaardwaarde is  true . De ruwe modus kan de indexeringssnelheid aanzienlijk verhogen, maar de normale modus verbetert de opmaak van de geëxtraheerde tekst.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of de ruwe modus wordt gebruikt voor teksteextractie indien mogelijk. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Haalt de opties op voor het indexeren van metagegevensvelden.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Haalt de opties op voor OCR-verwerking en het indexeren van herkende tekst.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Haalt de afbeeldingsindexeringsopties op voor omgekeerd zoeken naar afbeeldingen.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
