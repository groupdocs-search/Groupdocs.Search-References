---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement de changement de progression de l'opération d'optimisation."
type: docs
weight: 15
url: /fr/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Représente les arguments de l'événement de changement de progression de l'opération d'optimisation.

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Obtient l'index du nœud du réseau de recherche. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Obtient l'index du service du nœud du réseau de recherche. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Obtient le nombre de segments traités. |
|
|  | [getTotalSegments()](#getTotalSegments--) | Obtient le nombre total de segments à traiter. |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Obtient le nombre de segments traités.


**Returns:**
int - Le nombre de segments traités.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Obtient le nombre total de segments à traiter.


**Returns:**
int - Le nombre total de segments à traiter.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Obtient le pourcentage de la progression.


**Returns:**
double - Le pourcentage de la progression.

