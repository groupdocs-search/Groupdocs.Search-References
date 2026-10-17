---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement de changement de progression de l'opération d'indexation."
type: docs
weight: 14
url: /fr/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Représente les arguments de l'événement de changement de progression de l'opération d'indexation.

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Obtient l'index du nœud du réseau de recherche. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Obtient l'index du service du nœud du réseau de recherche. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Obtient le nombre de documents traités. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | Obtient le nombre total de documents à traiter. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Obtient le pourcentage de la progression. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Obtient l'index du nœud du réseau de recherche.


**Returns:**
int - L'index du nœud du réseau de recherche.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Obtient l'index du service du nœud du réseau de recherche.


**Returns:**
int - L'index du service du nœud du réseau de recherche.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Obtient le nombre de documents traités.


**Returns:**
int - Le nombre de documents traités.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Obtient le nombre total de documents à traiter.


**Returns:**
int - Le nombre total de documents à traiter.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Obtient le pourcentage de la progression.


**Returns:**
double - Le pourcentage de la progression.

