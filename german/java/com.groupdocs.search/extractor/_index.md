---
title: "Extractor"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein Werkzeug zur vorläufigen Datenerfassung aus Dokumenten dar, um die Phase der nachfolgenden schnellen Indizierung zu trennen."
type: docs
weight: 16
url: /de/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Stellt ein Werkzeug zur vorläufigen Datenerfassung aus Dokumenten dar, um die Phase der nachfolgenden schnellen Indizierung zu trennen.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Extractor()](#Extractor--) | Initialisiert eine neue Instanz der  Extractor  Klasse. |
|
## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Tritt auf, wenn ein Fehler während einer Extraktor-Operation auftritt. |
|
|  | [ImagePreparing](#ImagePreparing) | Tritt auf, wenn ein Bild für die Indizierung vorbereitet wird. |
|
|  | [PasswordRequired](#PasswordRequired) | Tritt auf, wenn ein Dokument ein Passwort zum Öffnen benötigt. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getSettings()](#getSettings--) | Ruft die Extraktor-Einstellungen ab. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Extrahiert Daten aus einem Dokument. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Initialisiert eine neue Instanz der  Extractor  Klasse.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Tritt auf, wenn ein Fehler während einer Extraktor-Operation auftritt.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Tritt auf, wenn ein Bild für die Indizierung vorbereitet wird.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Tritt auf, wenn ein Dokument ein Passwort zum Öffnen benötigt.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Ruft die Extraktor-Einstellungen ab.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Extrahiert Daten aus einem Dokument.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | Das Dokument aus dem Dateisystem, Stream oder einer Struktur. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | Die Extraktionsoptionen. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| message | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| documentKey | java.lang.String |  |
| innerPath | java.lang.String[] |  |
| imageIndex | int |  |
| frames | [ImageFrame\[\]](../../com.groupdocs.search.common/imageframe) |  |
| stream | java.io.InputStream |  |

### raisePasswordRequiredPublic(String filePath) {#raisePasswordRequiredPublic-java.lang.String-}
```
public final String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
