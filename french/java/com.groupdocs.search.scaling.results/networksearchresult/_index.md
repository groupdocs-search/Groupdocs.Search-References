---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un résultat de recherche correspondant à une requête de recherche."
type: docs
weight: 14
url: /fr/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Représente un résultat de recherche correspondant à une requête de recherche.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Obtient le nombre de documents trouvés. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtient le nombre total d'occurrences trouvées. |
|
|  | [getTruncated()](#getTruncated--) | Obtient une valeur indiquant que le résultat est tronqué. |
|
|  | [getWarnings()](#getWarnings--) | Obtient des avertissements décrivant le résultat. |
|
|  | [getStartTime()](#getStartTime--) | Obtient l'heure de début de la recherche. |
|
|  | [getEndTime()](#getEndTime--) | Obtient l'heure de fin de la recherche. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Obtient la durée de la recherche en secondes. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Obtient le document trouvé par indice. |
|
|  | [iterator()](#iterator--) | Renvoie un itérateur qui parcourt la collection des documents trouvés. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Obtient un jeton de recherche par bloc pour rechercher le bloc suivant. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Obtient l'indice du nœud à partir duquel le résultat a été reçu. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Obtient le nombre de documents trouvés.


**Returns:**
int - Le nombre de documents trouvés.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Obtient le nombre total d'occurrences trouvées.


**Returns:**
int - Le nombre total d'occurrences trouvées.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Obtient une valeur indiquant que le résultat est tronqué.


**Returns:**
boolean - Une valeur indiquant que le résultat est tronqué.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Obtient des avertissements décrivant le résultat.


**Returns:**
java.lang.String - Des avertissements décrivant le résultat.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Obtient l'heure de début de la recherche.


**Returns:**
java.util.Date - L'heure de début de la recherche.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Obtient l'heure de fin de la recherche.


**Returns:**
java.util.Date - L'heure de fin de la recherche.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Obtient la durée de la recherche en secondes.


**Returns:**
double - La durée de la recherche en secondes.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Obtient le document trouvé par indice.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | index | int | L'indice d'un document trouvé. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Renvoie un itérateur qui parcourt la collection des documents trouvés.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - Un itérateur qui peut être utilisé pour parcourir la collection des documents trouvés.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Obtient un jeton de recherche par bloc pour rechercher le bloc suivant.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Obtient l'indice du nœud à partir duquel le résultat a été reçu.


**Returns:**
int - L'indice du nœud à partir duquel le résultat a été reçu.

