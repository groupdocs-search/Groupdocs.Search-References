---
title: "NetworkFoundDocument"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un documento encontrado en la red de búsqueda."
type: docs
weight: 11
url: /es/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Representa un documento encontrado en la red de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Obtiene el documento encontrado. |
|
|  | [getShardIndex()](#getShardIndex--) | Obtiene el índice del fragmento. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Obtiene el documento encontrado.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Obtiene el índice del fragmento.


**Returns:**
int - El índice del fragmento.

