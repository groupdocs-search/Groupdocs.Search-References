---
title: "Extractor"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un outil d'extraction préliminaire de données à partir de documents afin de séparer l'étape d'indexation rapide ultérieure."
type: docs
weight: 16
url: /fr/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Représente un outil d'extraction préliminaire de données à partir de documents afin de séparer l'étape d'indexation rapide ultérieure.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [Extractor()](#Extractor--) | Initialise une nouvelle instance de la classe Extractor. |
|
## Fields

| Field | Description |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Se produit lorsqu'une erreur survient lors d'une opération d'extracteur. |
|
|  | [ImagePreparing](#ImagePreparing) | Se produit lorsqu'une image doit être préparée pour l'indexation. |
|
|  | [PasswordRequired](#PasswordRequired) | Se produit lorsqu'un document nécessite un mot de passe pour être ouvert. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getSettings()](#getSettings--) | Obtient les paramètres de l'extracteur. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Extrait des données d'un document. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Initialise une nouvelle instance de la classe Extractor.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Se produit lorsqu'une erreur survient lors d'une opération d'extracteur.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Se produit lorsqu'une image doit être préparée pour l'indexation.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Se produit lorsqu'un document nécessite un mot de passe pour être ouvert.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Obtient les paramètres de l'extracteur.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Extrait des données d'un document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | Le document provenant du système de fichiers, du flux ou de la structure. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | Les options d'extraction. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| message | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Paramètre | Type | Description |
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
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
