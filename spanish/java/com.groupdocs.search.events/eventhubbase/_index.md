---
title: "EventHubBase"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "La clase abstracta base para los concentradores de eventos."
type: docs
weight: 13
url: /es/java/com.groupdocs.search.events/eventhubbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class EventHubBase
```

La clase abstracta base para los concentradores de eventos.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [EventHubBase()](#EventHubBase--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### EventHubBase() {#EventHubBase--}
```
public EventHubBase()
```


### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public abstract void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| message | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public abstract void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
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
public abstract String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
