---
title: "UpdateOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för uppdateringsoperationen."
type: docs
weight: 43
url: /sv/java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

Tillhandahåller alternativ för uppdateringsoperationen.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)
* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [UpdateOptions()](#UpdateOptions--) | Initierar en ny instans av klassen  UpdateOptions  . |
|
|  | [UpdateOptions(Object data)](#UpdateOptions-java.lang.Object-) | Initierar en ny instans av klassen  UpdateOptions  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getThreads()](#getThreads--) | Hämtar antalet trådar som används för indexering. |
|
|  | [setThreads(int value)](#setThreads-int-) | Ställer in antalet trådar som används för indexering. |
|
|  | [isAsync()](#isAsync--) | Hämtar flaggan för asynkron utförande av operationen. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Ställer in flaggan för asynkron utförande av operationen. |
|
|  | [getCancellation()](#getCancellation--) | Hämtar objektet för avbrytning av operationen. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Ställer in objektet för avbrytning av operationen. |
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
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


Initierar en ny instans av klassen  UpdateOptions  .


### UpdateOptions(Object data) {#UpdateOptions-java.lang.Object-}
```
public UpdateOptions(Object data)
```


Initierar en ny instans av klassen  UpdateOptions  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | java.lang.Object | Den serialiserade datan. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Hämtar antalet trådar som används för indexering. Standardvärdet är  1 .


**Returns:**
int - Antalet trådar som används för indexering.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Ställer in antalet trådar som används för indexering. Standardvärdet är  1 .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Antalet trådar som används för indexering. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Hämtar flaggan för asynkron utförande av operationen. Standardvärdet är  false .


**Returns:**
boolean - Flaggan för asynkron utförande av operationen.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Ställer in flaggan för asynkron utförande av operationen. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Flaggan för asynkron utförande av operationen. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Hämtar objektet för avbrytning av operationen. Standardvärdet är  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Ställer in objektet för avbrytning av operationen. Standardvärdet är  null .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Objektet för avbrytning av operationen. |
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
