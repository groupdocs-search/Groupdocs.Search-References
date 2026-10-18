---
title: "ExtractionOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för att extrahera data från dokument."
type: docs
weight: 18
url: /sv/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Tillhandahåller alternativ för att extrahera data från dokument.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | Initierar en ny instans av  ExtractionOptions  klassen. |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Initierar en ny instans av  ExtractionOptions  klassen. |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Initierar en ny instans av  ExtractionOptions  klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Hämtar den anpassade textutdragaren. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Ställer in eller ställer in den anpassade textutdragaren. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Hämtar ett värde som indikerar om kodning ska upptäckas automatiskt eller inte. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Ställer in ett värde som indikerar om kodning ska upptäckas automatiskt eller inte. |
|
|  | [getEncoding()](#getEncoding--) | Hämtar kodningen som används för att extrahera text från textdokument. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Ställer in kodningen som används för att extrahera text från textdokument. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Hämtar ett värde som indikerar om råläge används för textutvinning om möjligt. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Ställer in ett värde som indikerar om råläge används för textutvinning om möjligt. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Hämtar alternativen för indexering av metadatafält. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Hämtar alternativen för OCR‑behandling och indexering av igenkänd text. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Hämtar bildindexeringsalternativen för omvänd bildsökning. |
|
| [getCore()](#getCore--) |  |
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Initierar en ny instans av  ExtractionOptions  klassen.


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Initierar en ny instans av  ExtractionOptions  klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | java.lang.Object | Den serialiserade datan. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Initierar en ny instans av  ExtractionOptions  klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Alternativen. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Den anpassade extrahören. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR‑anslutningen. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Hämtar den anpassade textutdragaren. Standardvärdet är  null .


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Ställer in eller ställer in den anpassade textutdragaren. Standardvärdet är  null .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Den anpassade textutdragaren. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Hämtar ett värde som indikerar om kodning ska upptäckas automatiskt eller inte. Standardvärdet är  false .


**Returns:**
boolean - Ett värde som indikerar om kodning ska upptäckas automatiskt eller inte.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Ställer in ett värde som indikerar om kodning ska upptäckas automatiskt eller inte. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om kodning ska upptäckas automatiskt eller inte. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Hämtar kodningen som används för att extrahera text från textdokument. Standardvärdet är  null , vilket betyder att standardkodningen UTF-8 används. Om AutoDetectEncoding är  true  används detta värde som standardkodning.


**Returns:**
java.lang.String - Kodningen som används för att extrahera text från textdokument.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Ställer in kodningen som används för att extrahera text från textdokument. Standardvärdet är  null , vilket betyder att standardkodningen UTF-8 används. Om AutoDetectEncoding är  true  används detta värde som standardkodning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Kodningen som används för att extrahera text från textdokument. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Hämtar ett värde som indikerar om råläge används för textutvinning om möjligt. Standardvärdet är  true . Råläget kan avsevärt öka indexeringshastigheten, men normalt läge förbättrar formateringen av den extraherade texten.


**Returns:**
boolean - Ett värde som indikerar om råläge används för textutvinning om möjligt.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Ställer in ett värde som indikerar om råläge används för textutvinning om möjligt. Standardvärdet är  true . Råläget kan avsevärt öka indexeringshastigheten, men normalt läge förbättrar formateringen av den extraherade texten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om råläge används för textutvinning om möjligt. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Hämtar alternativen för indexering av metadatafält.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Hämtar alternativen för OCR‑behandling och indexering av igenkänd text.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Hämtar bildindexeringsalternativen för omvänd bildsökning.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
