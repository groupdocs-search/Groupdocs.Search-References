---
title: "TextOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för att hämta dokumenttext från ett index."
type: docs
weight: 41
url: /sv/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Tillhandahåller alternativ för att hämta dokumenttext från ett index.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | Initierar en ny instans av klassen  TextOptions . |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | Initierar en ny instans av klassen  TextOptions . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Hämtar den anpassade textextraktorn som användes för indexering. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Ställer in den anpassade textextraktorn som användes för indexering. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Hämtar de ytterligare dokumentfälten som användes för indexering. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Ställer in de ytterligare dokumentfälten som användes för indexering. |
|
|  | [getCancellation()](#getCancellation--) | Hämtar avbokningsobjektet. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Ställer in avbokningsobjektet. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Hämtar ett värde som indikerar om Head-taggen genereras i den utgående HTML:en. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Ställer in ett värde som indikerar om Head-taggen genereras i den utgående HTML:en. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Initierar en ny instans av klassen  TextOptions .


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


Initierar en ny instans av klassen  TextOptions .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | java.lang.Object | Den serialiserade datan. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Hämtar den anpassade textutdragaren som användes för indexering. Standardvärdet är  null . Observera att detta värde endast används om dokumenttexten inte sparades i indexet.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Ställer in den anpassade textutdragaren som användes för indexering. Standardvärdet är  null . Observera att detta värde endast används om dokumenttexten inte sparades i indexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Den anpassade textutdragaren som användes för indexering. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Hämtar de ytterligare dokumentfälten som användes för indexering. Standardvärdet är  null . Observera att detta värde endast används om dokumenttexten inte sparades i indexet.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De ytterligare dokumentfälten som användes för indexering.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Ställer in de ytterligare dokumentfälten som användes för indexering. Standardvärdet är  null . Observera att detta värde endast används om dokumenttexten inte sparades i indexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | De ytterligare dokumentfälten som användes för indexering. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Hämtar avbokningsobjektet. Standardvärdet är  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Ställer in avbokningsobjektet. Standardvärdet är  null .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Avbrytningsobjektet. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Hämtar ett värde som indikerar om Head-taggen genereras i den utgående HTML:en. Standardvärdet är  true .


**Returns:**
boolean - Ett värde som indikerar om Head-taggen genereras i den utgående HTML:en.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Ställer in ett värde som indikerar om Head-taggen genereras i den utgående HTML:en. Standardvärdet är  true .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om Head-taggen genereras i den utgående HTML:en. |
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
