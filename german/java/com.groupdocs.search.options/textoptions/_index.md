---
title: "TextOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Optionen zum Abrufen von Dokumenttext aus einem Index bereit."
type: docs
weight: 41
url: /de/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Stellt Optionen zum Abrufen von Dokumenttext aus einem Index bereit.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | Initialisiert eine neue Instanz der  TextOptions  Klasse. |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | Initialisiert eine neue Instanz der  TextOptions  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Ruft den benutzerdefinierten Text-Extraktor ab, der für die Indizierung verwendet wurde. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Legt den benutzerdefinierten Text-Extraktor fest, der für die Indizierung verwendet wurde. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Ruft die zusätzlichen Dokumentfelder ab, die für die Indizierung verwendet wurden. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Legt die zusätzlichen Dokumentfelder fest, die für die Indizierung verwendet wurden. |
|
|  | [getCancellation()](#getCancellation--) | Ruft das Abbruchobjekt ab. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Legt das Abbruchobjekt fest. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Ruft einen Wert ab, der angibt, ob das Head-Tag im ausgegebenen HTML erzeugt wird. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Legt einen Wert fest, der angibt, ob das Head-Tag im ausgegebenen HTML erzeugt wird. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Initialisiert eine neue Instanz der  TextOptions  Klasse.


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


Initialisiert eine neue Instanz der  TextOptions  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | java.lang.Object | Die serialisierten Daten. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Ruft den benutzerdefinierten Text-Extraktor ab, der für die Indizierung verwendet wurde. Der Standardwert ist null. Hinweis: Dieser Wert wird nur verwendet, wenn der Dokumenttext nicht im Index gespeichert wurde.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Legt den benutzerdefinierten Text-Extraktor fest, der für die Indizierung verwendet wurde. Der Standardwert ist null. Hinweis: Dieser Wert wird nur verwendet, wenn der Dokumenttext nicht im Index gespeichert wurde.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Der benutzerdefinierte Text-Extraktor, der für die Indizierung verwendet wurde. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Ruft die zusätzlichen Dokumentfelder ab, die für die Indizierung verwendet wurden. Der Standardwert ist null. Hinweis: Dieser Wert wird nur verwendet, wenn der Dokumenttext nicht im Index gespeichert wurde.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Die zusätzlichen Dokumentfelder, die für die Indizierung verwendet wurden.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Legt die zusätzlichen Dokumentfelder fest, die für die Indizierung verwendet wurden. Der Standardwert ist null. Hinweis: Dieser Wert wird nur verwendet, wenn der Dokumenttext nicht im Index gespeichert wurde.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Die zusätzlichen Dokumentfelder, die für die Indizierung verwendet wurden. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Ruft das Abbruchobjekt ab. Der Standardwert ist null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Legt das Abbruchobjekt fest. Der Standardwert ist null.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Das Abbruchobjekt. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Ruft einen Wert ab, der angibt, ob das Head-Tag im ausgegebenen HTML erzeugt wird. Der Standardwert ist true.


**Returns:**
boolean - Ein Wert, der angibt, ob das Head-Tag im ausgegebenen HTML erzeugt wird.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Legt einen Wert fest, der angibt, ob das Head-Tag im ausgegebenen HTML erzeugt wird. Der Standardwert ist true.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob das Head-Tag im ausgegebenen HTML erzeugt wird. |
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
