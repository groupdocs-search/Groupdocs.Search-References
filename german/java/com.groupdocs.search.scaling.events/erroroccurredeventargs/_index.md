---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, wenn in einem der Knoten des Suchnetzwerks ein Fehler auftritt."
type: docs
weight: 13
url: /de/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Stellt Argumente für das Ereignis dar, wenn in einem der Knoten des Suchnetzwerks ein Fehler auftritt.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Ermittelt den Index des Suchnetzwerk-Knotens. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Ermittelt den Index des Suchnetzwerk-Knoten-Dienstes. |
|
|  | [getMessage()](#getMessage--) | Ermittelt die Fehlermeldung. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Ermittelt den Index des Suchnetzwerk-Knotens.


**Returns:**
int - Der Index des Suchnetzwerk-Knotens.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Ermittelt den Index des Suchnetzwerk-Knoten-Dienstes.


**Returns:**
int - Der Index des Suchnetzwerk-Knoten-Dienstes.

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Ermittelt die Fehlermeldung.


**Returns:**
java.lang.String - Die Fehlermeldung.

