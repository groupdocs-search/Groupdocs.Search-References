---
title: "DocumentIndexedEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di completamento dell'indicizzazione di un documento."
type: docs
weight: 12
url: /it/java/com.groupdocs.search.scaling.events/documentindexedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentIndexedEventArgs extends EventArgs
```

Rappresenta gli argomenti per l'evento di completamento dell'indicizzazione di un documento.

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Restituisce l'indice della shard. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Restituisce la chiave del documento. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Restituisce l'indice della shard.


**Returns:**
int - L'indice della shard.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Restituisce la chiave del documento.


**Returns:**
java.lang.String - La chiave del documento.

