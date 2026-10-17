---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement de mise à jour de la progression de l'opération d'indexation."
type: docs
weight: 19
url: /fr/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Représente les arguments de l'événement de mise à jour de la progression de l'opération d'indexation.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | Obtient le nombre total de segments à traiter. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Obtient le nombre de segments traités. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Obtient le pourcentage de la progression. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Obtient le nombre total de segments à traiter.


**Returns:**
int - Le nombre total de segments à traiter.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Obtient le nombre de segments traités.


**Returns:**
int - Le nombre de segments traités.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Obtient le pourcentage de la progression.


**Returns:**
double - Le pourcentage de la progression.

