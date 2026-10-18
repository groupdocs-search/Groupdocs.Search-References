---
title: "NetworkDocumentInfo"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un descriptor para un documento indexado en la red de búsqueda."
type: docs
weight: 10
url: /es/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Representa un descriptor para un documento indexado en la red de búsqueda.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Obtiene el descriptor de un documento indexado. |
|
|  | [getShardIndex()](#getShardIndex--) | Obtiene el índice del fragmento. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Obtiene el descriptor de un documento indexado.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Obtiene el índice del fragmento.


**Returns:**
int - El índice del fragmento.

