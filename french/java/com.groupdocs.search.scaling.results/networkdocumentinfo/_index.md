---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un descripteur pour un document indexé dans le réseau de recherche."
type: docs
weight: 10
url: /fr/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Représente un descripteur pour un document indexé dans le réseau de recherche.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Obtient le descripteur d'un document indexé. |
|
|  | [getShardIndex()](#getShardIndex--) | Obtient l'index de la partition. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Obtient le descripteur d'un document indexé.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Obtient l'index de la partition.


**Returns:**
int - L'index de la partition.

