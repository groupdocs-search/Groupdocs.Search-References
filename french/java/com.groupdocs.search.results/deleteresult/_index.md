---
title: "DeleteResult"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente le résultat de l'opération de suppression de fichiers ou dossiers indexés d'un index."
type: docs
weight: 10
url: /fr/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Représente le résultat de l'opération de suppression de fichiers ou dossiers indexés d'un index.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Renvoie les résultats de la suppression de chaque chemin. |
|
|  | [getTotalCount()](#getTotalCount--) | Renvoie le nombre total de chemins à supprimer. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Renvoie le nombre de chemins supprimés avec succès. |
|
|  | [getFailedCount()](#getFailedCount--) | Renvoie le nombre de chemins non supprimés en raison d'erreurs. |
|
|  | [getErrors()](#getErrors--) | Renvoie les descriptions des erreurs de suppression. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Renvoie les résultats de la suppression de chaque chemin.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - Les résultats de la suppression de chaque chemin.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Renvoie le nombre total de chemins à supprimer.


**Returns:**
int - Le nombre total de chemins à supprimer.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Renvoie le nombre de chemins supprimés avec succès.


**Returns:**
int - Le nombre de chemins supprimés avec succès.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Renvoie le nombre de chemins non supprimés en raison d'erreurs.


**Returns:**
int - Le nombre de chemins non supprimés en raison d'erreurs.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Renvoie les descriptions des erreurs de suppression.


**Returns:**
java.lang.String[] - Descriptions des erreurs de suppression.

