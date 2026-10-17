---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente la classe de base des arguments d'événement."
type: docs
weight: 10
url: /fr/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Représente la classe de base des arguments d'événement.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getTime()](#getTime--) | Obtient l'heure d'un événement. |
|
|  | [getIndexId()](#getIndexId--) | Obtient l'ID de l'index. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Obtient le dossier de l'index. |
|
|  | [getStatus()](#getStatus--) | Obtient le statut de l'index. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Obtient l'heure d'un événement.


**Returns:**
java.util.Date - L'heure d'un événement.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Obtient l'ID de l'index.


**Returns:**
java.util.UUID - L'ID de l'index.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Obtient le dossier de l'index.


**Returns:**
java.lang.String - Le dossier de l'index.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Obtient le statut de l'index.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

