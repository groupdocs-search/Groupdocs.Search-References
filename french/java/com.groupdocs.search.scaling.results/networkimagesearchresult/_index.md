---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un résultat de recherche d'image correspondant à une image de recherche."
type: docs
weight: 12
url: /fr/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Représente un résultat de recherche d'image correspondant à une image de recherche.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Obtient le nombre d'images trouvées. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Obtient l'image trouvée par indice. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Obtient un jeton de recherche d'image par bloc pour rechercher le bloc suivant. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Obtient l'indice du nœud à partir duquel le résultat a été reçu. |
|
|  | [getShardIndex()](#getShardIndex--) | Obtient l'indice du fragment à partir duquel le résultat a été reçu. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Obtient le nombre d'images trouvées.


**Returns:**
int - Le nombre d'images trouvées.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Obtient l'image trouvée par indice.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | index | int | L'indice d'une image trouvée. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Obtient un jeton de recherche d'image par bloc pour rechercher le bloc suivant.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Obtient l'indice du nœud à partir duquel le résultat a été reçu.


**Returns:**
int - L'indice du nœud à partir duquel le résultat a été reçu.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Obtient l'indice du fragment à partir duquel le résultat a été reçu.


**Returns:**
int - L'indice du fragment à partir duquel le résultat a été reçu.

