---
title: "UpdateOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Optionen für den Aktualisierungsvorgang bereit."
type: docs
weight: 43
url: /de/java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

Stellt Optionen für den Aktualisierungsvorgang bereit.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)
* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [UpdateOptions()](#UpdateOptions--) | Initialisiert eine neue Instanz der UpdateOptions-Klasse. |
|
|  | [UpdateOptions(Object data)](#UpdateOptions-java.lang.Object-) | Initialisiert eine neue Instanz der UpdateOptions-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getThreads()](#getThreads--) | Liest die Anzahl der für die Indizierung verwendeten Threads. |
|
|  | [setThreads(int value)](#setThreads-int-) | Setzt die Anzahl der für die Indizierung verwendeten Threads. |
|
|  | [isAsync()](#isAsync--) | Liest das Flag für die asynchrone Ausführung der Operation. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Setzt das Flag für die asynchrone Ausführung der Operation. |
|
|  | [getCancellation()](#getCancellation--) | Liest das Abbruchobjekt der Operation. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Setzt das Abbruchobjekt der Operation. |
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
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


Initialisiert eine neue Instanz der UpdateOptions-Klasse.


### UpdateOptions(Object data) {#UpdateOptions-java.lang.Object-}
```
public UpdateOptions(Object data)
```


Initialisiert eine neue Instanz der UpdateOptions-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | java.lang.Object | Die serialisierten Daten. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Gibt die Anzahl der für das Indizieren verwendeten Threads zurück. Der Standardwert ist  1 .


**Returns:**
int - Die Anzahl der für das Indizieren verwendeten Threads.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Legt die Anzahl der für das Indizieren verwendeten Threads fest. Der Standardwert ist  1 .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die Anzahl der für das Indizieren verwendeten Threads. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Gibt das Flag für die asynchrone Ausführung der Operation zurück. Der Standardwert ist  false .


**Returns:**
boolean - Das Flag für die asynchrone Ausführung der Operation.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Legt das Flag für die asynchrone Ausführung der Operation fest. Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Das Flag für die asynchrone Ausführung der Operation. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Gibt das Abbruchobjekt der Operation zurück. Der Standardwert ist  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Legt das Abbruchobjekt der Operation fest. Der Standardwert ist  null .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Das Abbruchobjekt der Operation. |
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
