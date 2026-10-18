---
title: "EventHubBase"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "La classe astratta base per i hub di eventi."
type: docs
weight: 13
url: /it/java/com.groupdocs.search.events/eventhubbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class EventHubBase
```

La classe astratta base per i hub di eventi.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [EventHubBase()](#EventHubBase--) |  |
## Metodi

| Metodo | Descrizione |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| messaggio | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public abstract void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
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
public abstract String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
