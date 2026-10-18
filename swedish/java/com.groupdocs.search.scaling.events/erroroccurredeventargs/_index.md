---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelsen när ett fel uppstår i en av noderna i söknätverket."
type: docs
weight: 13
url: /sv/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Representerar argument för händelsen när ett fel uppstår i en av noderna i söknätverket.

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Hämtar index för söknätsnod. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Hämtar index för söknätsnodtjänst. |
|
|  | [getMessage()](#getMessage--) | Hämtar felmeddelandet. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Hämtar index för söknätsnod.


**Returns:**
int - Index för söknätsnod.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Hämtar index för söknätsnodtjänst.


**Returns:**
int - Index för söknätsnodtjänst.

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Hämtar felmeddelandet.


**Returns:**
java.lang.String - Felmeddelandet.

