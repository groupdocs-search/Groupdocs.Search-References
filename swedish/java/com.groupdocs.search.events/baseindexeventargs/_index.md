---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar basklassen för händelseargument."
type: docs
weight: 10
url: /sv/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Representerar basklassen för händelseargument.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getTime()](#getTime--) | Hämtar tiden för en händelse. |
|
|  | [getIndexId()](#getIndexId--) | Hämtar index‑ID:t. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Hämtar index‑mappen. |
|
|  | [getStatus()](#getStatus--) | Hämtar index‑statusen. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Hämtar tiden för en händelse.


**Returns:**
java.util.Date - Tiden för en händelse.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Hämtar index‑ID:t.


**Returns:**
java.util.UUID - Index‑ID:t.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Hämtar index‑mappen.


**Returns:**
java.lang.String - Index‑mappen.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Hämtar index‑statusen.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

