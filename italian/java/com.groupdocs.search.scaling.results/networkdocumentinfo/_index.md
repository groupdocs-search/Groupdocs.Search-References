---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un descrittore per un documento indicizzato nella rete di ricerca."
type: docs
weight: 10
url: /it/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Rappresenta un descrittore per un documento indicizzato nella rete di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Ottiene il descrittore per un documento indicizzato. |
|
|  | [getShardIndex()](#getShardIndex--) | Restituisce l'indice della shard. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Ottiene il descrittore per un documento indicizzato.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Restituisce l'indice della shard.


**Returns:**
int - L'indice della shard.

