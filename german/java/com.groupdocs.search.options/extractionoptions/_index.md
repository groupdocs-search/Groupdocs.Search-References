---
title: "ExtractionOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Bietet Optionen zum Extrahieren von Daten aus Dokumenten."
type: docs
weight: 18
url: /de/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Bietet Optionen zum Extrahieren von Daten aus Dokumenten.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | Initialisiert eine neue Instanz der  ExtractionOptions  Klasse. |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Initialisiert eine neue Instanz der  ExtractionOptions  Klasse. |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Initialisiert eine neue Instanz der  ExtractionOptions  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Gibt den benutzerdefinierten Text‑Extraktor zurück. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Setzt oder ändert den benutzerdefinierten Text‑Extraktor. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Liest einen Wert, der angibt, ob die Kodierung automatisch erkannt werden soll oder nicht. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Setzt einen Wert, der angibt, ob die Kodierung automatisch erkannt werden soll oder nicht. |
|
|  | [getEncoding()](#getEncoding--) | Liest die Kodierung, die zum Extrahieren von Text aus Textdokumenten verwendet wird. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Legt die Kodierung fest, die zum Extrahieren von Text aus Textdokumenten verwendet wird. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Gibt einen Wert zurück, der angibt, ob der Rohmodus für die Textextraktion verwendet wird, falls möglich. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Legt einen Wert fest, der angibt, ob der Rohmodus für die Textextraktion verwendet wird, falls möglich. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Gibt die Optionen für das Indizieren von Metadatenfeldern zurück. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Gibt die Optionen für die OCR-Verarbeitung und das Indizieren von erkanntem Text zurück. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Gibt die Bildindizierungsoptionen für die umgekehrte Bildsuche zurück. |
|
| [getCore()](#getCore--) |  |
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Initialisiert eine neue Instanz der  ExtractionOptions  Klasse.


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Initialisiert eine neue Instanz der  ExtractionOptions  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | java.lang.Object | Die serialisierten Daten. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Initialisiert eine neue Instanz der  ExtractionOptions  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Die Optionen. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Der benutzerdefinierte Extraktor. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Der OCR‑Connector. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Gibt den benutzerdefinierten Text‑Extraktor zurück. Der Standardwert ist  null .


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Setzt oder ändert den benutzerdefinierten Text‑Extraktor. Der Standardwert ist  null .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Der benutzerdefinierte Text‑Extraktor. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Gibt einen Wert zurück, der angibt, ob die Kodierung automatisch erkannt werden soll oder nicht. Der Standardwert ist  false .


**Returns:**
boolean - Ein Wert, der angibt, ob die Kodierung automatisch erkannt werden soll oder nicht.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Legt einen Wert fest, der angibt, ob die Kodierung automatisch erkannt werden soll oder nicht. Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob die Kodierung automatisch erkannt werden soll oder nicht. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Gibt die Kodierung zurück, die zum Extrahieren von Text aus Textdokumenten verwendet wird. Der Standardwert ist  null , was bedeutet, dass die Standardkodierung UTF-8 verwendet wird. Wenn AutoDetectEncoding  true  ist, wird dieser Wert als Standardkodierung verwendet.


**Returns:**
java.lang.String - Die Kodierung, die zum Extrahieren von Text aus Textdokumenten verwendet wird.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Legt die Kodierung fest, die zum Extrahieren von Text aus Textdokumenten verwendet wird. Der Standardwert ist  null , was bedeutet, dass die Standardkodierung UTF-8 verwendet wird. Wenn AutoDetectEncoding  true  ist, wird dieser Wert als Standardkodierung verwendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Die Kodierung, die zum Extrahieren von Text aus Textdokumenten verwendet wird. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Gibt einen Wert zurück, der angibt, ob der Rohmodus nach Möglichkeit für die Textextraktion verwendet wird. Der Standardwert ist true. Der Rohmodus kann die Indexierungsgeschwindigkeit erheblich erhöhen, aber der Normalmodus verbessert die Formatierung des extrahierten Textes.


**Returns:**
boolean - Ein Wert, der angibt, ob der Rohmodus nach Möglichkeit für die Textextraktion verwendet wird.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Setzt einen Wert, der angibt, ob der Rohmodus nach Möglichkeit für die Textextraktion verwendet wird. Der Standardwert ist true. Der Rohmodus kann die Indexierungsgeschwindigkeit erheblich erhöhen, aber der Normalmodus verbessert die Formatierung des extrahierten Textes.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob der Rohmodus nach Möglichkeit für die Textextraktion verwendet wird. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Gibt die Optionen für das Indizieren von Metadatenfeldern zurück.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Gibt die Optionen für die OCR-Verarbeitung und das Indizieren von erkanntem Text zurück.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Gibt die Bildindizierungsoptionen für die umgekehrte Bildsuche zurück.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
