---
title: "Extractor"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa una herramienta para la extracción preliminar de datos de documentos, separando la etapa de indexación rápida posterior."
type: docs
weight: 16
url: /es/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Representa una herramienta para la extracción preliminar de datos de documentos, separando la etapa de indexación rápida posterior.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Extractor()](#Extractor--) | Inicializa una nueva instancia de la clase  Extractor  . |
|
## Campos

| Campo | Descripción |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Ocurre cuando se produce un error durante una operación del extractor. |
|
|  | [ImagePreparing](#ImagePreparing) | Ocurre cuando una imagen está a punto de prepararse para indexarse. |
|
|  | [PasswordRequired](#PasswordRequired) | Ocurre cuando un documento requiere contraseña para abrirse. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getSettings()](#getSettings--) | Obtiene la configuración del extractor. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Extrae datos de un documento. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Inicializa una nueva instancia de la clase  Extractor  .


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Ocurre cuando se produce un error durante una operación del extractor.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Ocurre cuando una imagen está a punto de prepararse para indexarse.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Ocurre cuando un documento requiere contraseña para abrirse.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Obtiene la configuración del extractor.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Extrae datos de un documento.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | El documento del sistema de archivos, flujo o estructura. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | Las opciones de extracción. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| message | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
