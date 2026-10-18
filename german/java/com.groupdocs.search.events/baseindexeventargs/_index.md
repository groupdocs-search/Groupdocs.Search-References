---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Basisklasse für Ereignisargumente dar."
type: docs
weight: 10
url: /de/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Stellt die Basisklasse für Ereignisargumente dar.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getTime()](#getTime--) | Ermittelt die Zeit eines Ereignisses. |
|
|  | [getIndexId()](#getIndexId--) | Ermittelt die Index-ID. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Ermittelt den Indexordner. |
|
|  | [getStatus()](#getStatus--) | Ermittelt den Indexstatus. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Ermittelt die Zeit eines Ereignisses.


**Returns:**
java.util.Date - Die Zeit eines Ereignisses.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Ermittelt die Index-ID.


**Returns:**
java.util.UUID - Die Index-ID.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Ermittelt den Indexordner.


**Returns:**
java.lang.String - Der Indexordner.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Ermittelt den Indexstatus.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

