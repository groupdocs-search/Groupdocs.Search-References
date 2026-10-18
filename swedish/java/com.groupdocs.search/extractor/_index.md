---
title: "Extractor"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett verktyg för preliminär dataextraktion från dokument för att separera steget av efterföljande snabb indexering."
type: docs
weight: 16
url: /sv/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Representerar ett verktyg för preliminär dataextraktion från dokument för att separera steget av efterföljande snabb indexering.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Extractor()](#Extractor--) | Initierar en ny instans av  Extractor  klassen. |
|
## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Uppstår när ett fel inträffar under en extraheringsoperation. |
|
|  | [ImagePreparing](#ImagePreparing) | Uppstår när en bild ska förberedas för indexering. |
|
|  | [PasswordRequired](#PasswordRequired) | Uppstår när ett dokument kräver lösenord för att öppnas. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getSettings()](#getSettings--) | Hämtar extraherarens inställningar. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Extraherar data från ett dokument. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Initierar en ny instans av  Extractor  klassen.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Uppstår när ett fel inträffar under en extraheringsoperation.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Uppstår när en bild ska förberedas för indexering.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Uppstår när ett dokument kräver lösenord för att öppnas.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Hämtar extraherarens inställningar.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Extraherar data från ett dokument.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | Dokumentet från filsystem, ström eller struktur. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | Extraktionsalternativen. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| meddelande | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| documentKey | java.lang.String |  |
| innerPath | java.lang.String[] |  |
| imageIndex | int |  |
| frames | [ImageFrame\[\]](../../com.groupdocs.search.common/imageframe) |  |
| ström | java.io.InputStream |  |

### raisePasswordRequiredPublic(String filePath) {#raisePasswordRequiredPublic-java.lang.String-}
```
public final String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
