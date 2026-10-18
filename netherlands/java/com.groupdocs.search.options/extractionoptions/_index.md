---
title: "ExtractionOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor het extraheren van gegevens uit documenten."
type: docs
weight: 18
url: /nl/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Biedt opties voor het extraheren van gegevens uit documenten.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | Initialiseert een nieuw exemplaar van de  ExtractionOptions  klasse. |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Initialiseert een nieuw exemplaar van de  ExtractionOptions  klasse. |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Initialiseert een nieuw exemplaar van de  ExtractionOptions  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Haalt de aangepaste tekst-extractor op. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Stelt de aangepaste tekst-extractor in of stelt deze in. |
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
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Initialiseert een nieuw exemplaar van de  ExtractionOptions  klasse.


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Initialiseert een nieuw exemplaar van de  ExtractionOptions  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | gegevens | java.lang.Object | De geserialiseerde gegevens. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Initialiseert een nieuw exemplaar van de  ExtractionOptions  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | De opties. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | De aangepaste extractor. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | De OCR-connector. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Haalt de aangepaste tekst-extractor op. De standaardwaarde is  null .


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Stelt de aangepaste tekst-extractor in of stelt deze in. De standaardwaarde is  null .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | De aangepaste tekst-extractor. |
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
