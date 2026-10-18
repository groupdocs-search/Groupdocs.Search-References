---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un documento trovato nella rete di ricerca."
type: docs
weight: 11
url: /it/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Rappresenta un documento trovato nella rete di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Ottiene il documento trovato. |
|
|  | [getShardIndex()](#getShardIndex--) | Restituisce l'indice della shard. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Ottiene il documento trovato.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Restituisce l'indice della shard.


**Returns:**
int - L'indice della shard.

