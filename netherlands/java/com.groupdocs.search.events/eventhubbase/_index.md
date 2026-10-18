---
title: "EventHubBase"
second_title: "GroupDocs.Search for Java API-referentie"
description: "De abstracte basisklasse voor gebeurtenis‑hubs."
type: docs
weight: 13
url: /nl/java/com.groupdocs.search.events/eventhubbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class EventHubBase
```

De abstracte basisklasse voor gebeurtenis‑hubs.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [EventHubBase()](#EventHubBase--) |  |
## Methoden

| Methode | Beschrijving |
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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bericht | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public abstract void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
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
public abstract String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
