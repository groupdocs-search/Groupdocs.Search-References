---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta la classe base degli argomenti dell'evento."
type: docs
weight: 10
url: /it/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Rappresenta la classe base degli argomenti dell'evento.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getTime()](#getTime--) | Restituisce l'ora di un evento. |
|
|  | [getIndexId()](#getIndexId--) | Restituisce l'ID dell'indice. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Restituisce la cartella dell'indice. |
|
|  | [getStatus()](#getStatus--) | Restituisce lo stato dell'indice. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Restituisce l'ora di un evento.


**Returns:**
java.util.Date - L'ora di un evento.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Restituisce l'ID dell'indice.


**Returns:**
java.util.UUID - L'ID dell'indice.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Restituisce la cartella dell'indice.


**Returns:**
java.lang.String - La cartella dell'indice.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Restituisce lo stato dell'indice.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

