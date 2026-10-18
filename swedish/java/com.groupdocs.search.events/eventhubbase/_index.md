---
title: "EventHubBase"
second_title: "GroupDocs.Search för Java API-referens"
description: "Den abstrakta basklassen för händelsehubbar."
type: docs
weight: 13
url: /sv/java/com.groupdocs.search.events/eventhubbase/
---
**Inheritance:**
java.lang.Object
```
public abstract class EventHubBase
```

Den abstrakta basklassen för händelsehubbar.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [EventHubBase()](#EventHubBase--) |  |
## Metoder

| Metod | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| meddelande | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public abstract void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
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
public abstract String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
