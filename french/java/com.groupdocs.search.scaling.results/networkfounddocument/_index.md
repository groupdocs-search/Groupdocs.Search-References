---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un document trouvé dans le réseau de recherche."
type: docs
weight: 11
url: /fr/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Représente un document trouvé dans le réseau de recherche.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Obtient le document trouvé. |
|
|  | [getShardIndex()](#getShardIndex--) | Obtient l'index de la partition. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Obtient le document trouvé.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Obtient l'index de la partition.


**Returns:**
int - L'index de la partition.

