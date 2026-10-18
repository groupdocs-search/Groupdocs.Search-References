---
title: "TextOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor het ophalen van documenttekst uit een index."
type: docs
weight: 41
url: /nl/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Biedt opties voor het ophalen van documenttekst uit een index.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | Initialiseert een nieuwe instantie van de  TextOptions  klasse. |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | Initialiseert een nieuwe instantie van de  TextOptions  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Haalt de aangepaste tekstextractor op die werd gebruikt voor indexering. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Stelt de aangepaste tekstextractor in die werd gebruikt voor indexering. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Haalt de extra documentvelden op die werden gebruikt voor indexering. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Stelt de extra documentvelden in die werden gebruikt voor indexering. |
|
|  | [getCancellation()](#getCancellation--) | Haalt het annuleringsobject op. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Stelt het annuleringsobject in. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Haalt een waarde op die aangeeft of de Head-tag wordt gegenereerd in de uitvoer-HTML. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Stelt een waarde in die aangeeft of de Head-tag wordt gegenereerd in de uitvoer-HTML. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Initialiseert een nieuwe instantie van de  TextOptions  klasse.


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


Initialiseert een nieuwe instantie van de  TextOptions  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | gegevens | java.lang.Object | De geserialiseerde gegevens. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Haalt de aangepaste tekst-extractor op die werd gebruikt voor indexering. De standaardwaarde is null. Merk op dat deze waarde alleen wordt gebruikt als documenttekst niet in de index is opgeslagen.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Stelt de aangepaste tekst-extractor in die werd gebruikt voor indexering. De standaardwaarde is null. Merk op dat deze waarde alleen wordt gebruikt als documenttekst niet in de index is opgeslagen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | De aangepaste tekst-extractor die werd gebruikt voor indexering. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Haalt de extra documentvelden op die werden gebruikt voor indexering. De standaardwaarde is null. Merk op dat deze waarde alleen wordt gebruikt als documenttekst niet in de index is opgeslagen.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De extra documentvelden die werden gebruikt voor indexering.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Stelt de extra documentvelden in die werden gebruikt voor indexering. De standaardwaarde is null. Merk op dat deze waarde alleen wordt gebruikt als documenttekst niet in de index is opgeslagen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | De extra documentvelden die werden gebruikt voor indexering. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Haalt het annuleringsobject op. De standaardwaarde is null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Stelt het annuleringsobject in. De standaardwaarde is null.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Het annuleringsobject. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Haalt een waarde op die aangeeft of de Head-tag wordt gegenereerd in de uitvoer-HTML. De standaardwaarde is true.


**Returns:**
boolean - Een waarde die aangeeft of de Head-tag wordt gegenereerd in de uitvoer-HTML.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Stelt een waarde in die aangeeft of de Head-tag wordt gegenereerd in de uitvoer-HTML. De standaardwaarde is true.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of de Head-tag wordt gegenereerd in de uitvoer-HTML. |
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
