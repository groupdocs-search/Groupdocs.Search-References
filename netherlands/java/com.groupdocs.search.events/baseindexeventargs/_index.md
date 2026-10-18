---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de basisklasse van gebeurtenisargumenten voor."
type: docs
weight: 10
url: /nl/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Stelt de basisklasse van gebeurtenisargumenten voor.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getTime()](#getTime--) | Haalt de tijd van een gebeurtenis op. |
|
|  | [getIndexId()](#getIndexId--) | Haalt de index-ID op. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Haalt de indexmap op. |
|
|  | [getStatus()](#getStatus--) | Haalt de indexstatus op. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Haalt de tijd van een gebeurtenis op.


**Returns:**
java.util.Date - De tijd van een gebeurtenis.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Haalt de index-ID op.


**Returns:**
java.util.UUID - De index-ID.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Haalt de indexmap op.


**Returns:**
java.lang.String - De indexmap.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Haalt de indexstatus op.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

