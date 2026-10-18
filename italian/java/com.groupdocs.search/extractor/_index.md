---
title: "Extractor"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta uno strumento per l'estrazione preliminare dei dati dai documenti per separare la fase di indicizzazione rapida successiva."
type: docs
weight: 16
url: /it/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Rappresenta uno strumento per l'estrazione preliminare dei dati dai documenti per separare la fase di indicizzazione rapida successiva.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Extractor()](#Extractor--) | Inizializza una nuova istanza della classe  Extractor . |
|
## Fields

| Field | Descrizione |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Si verifica quando si verifica un errore durante un'operazione di extractor. |
|
|  | [ImagePreparing](#ImagePreparing) | Si verifica quando un'immagine sta per essere preparata per l'indicizzazione. |
|
|  | [PasswordRequired](#PasswordRequired) | Si verifica quando un documento richiede una password per l'apertura. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getSettings()](#getSettings--) | Ottiene le impostazioni dell'extractor. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Estrae dati da un documento. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Inizializza una nuova istanza della classe  Extractor .


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Si verifica quando si verifica un errore durante un'operazione di extractor.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Si verifica quando un'immagine sta per essere preparata per l'indicizzazione.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Si verifica quando un documento richiede una password per l'apertura.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Ottiene le impostazioni dell'extractor.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Estrae dati da un documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | Il documento dal file system, stream o struttura. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | Le opzioni di estrazione. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| messaggio | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
