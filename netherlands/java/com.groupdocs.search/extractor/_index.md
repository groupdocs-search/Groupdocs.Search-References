---
title: "Extractor"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een hulpmiddel voor voorlopige gegevensextractie uit documenten voor om de fase van daaropvolgende snelle indexering te scheiden."
type: docs
weight: 16
url: /nl/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Stelt een hulpmiddel voor voorlopige gegevensextractie uit documenten voor om de fase van daaropvolgende snelle indexering te scheiden.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Extractor()](#Extractor--) | Initialiseert een nieuw exemplaar van de Extractor-klasse. |
|
## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Treedt op wanneer er een fout optreedt tijdens een extractorbewerking. |
|
|  | [ImagePreparing](#ImagePreparing) | Treedt op wanneer een afbeelding wordt voorbereid voor indexering. |
|
|  | [PasswordRequired](#PasswordRequired) | Treedt op wanneer een document een wachtwoord vereist om te openen. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getSettings()](#getSettings--) | Haalt de extractorinstellingen op. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Extraheert gegevens uit een document. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Initialiseert een nieuw exemplaar van de Extractor-klasse.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Treedt op wanneer er een fout optreedt tijdens een extractorbewerking.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Treedt op wanneer een afbeelding wordt voorbereid voor indexering.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Treedt op wanneer een document een wachtwoord vereist om te openen.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Haalt de extractorinstellingen op.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Extraheert gegevens uit een document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | Het document van het bestandssysteem, stream of structuur. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | De extractie‑opties. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bericht | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Parameter | Type | Beschrijving |
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
