---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement de mise à jour de la progression de l'opération d'indexation."
type: docs
weight: 18
url: /fr/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Représente les arguments de l'événement de mise à jour de la progression de l'opération d'indexation.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | Obtient le nombre total de documents à traiter. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Obtient le nombre de documents traités avec succès. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Obtient le nombre de documents ignorés. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Obtient le pourcentage de la progression. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Obtient la clé du dernier document traité. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Obtient le chemin du dernier document traité. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Obtient le statut du dernier document traité. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Obtient le nombre total de documents à traiter.


**Returns:**
int - Le nombre total de documents à traiter.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Obtient le nombre de documents traités avec succès.


**Returns:**
int - Le nombre de documents traités avec succès.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Obtient le nombre de documents ignorés.


**Returns:**
int - Le nombre de documents ignorés.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Obtient le pourcentage de la progression.


**Returns:**
double - Le pourcentage de la progression.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Obtient la clé du dernier document traité.


**Returns:**
java.lang.String - La clé du dernier document traité.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Obtient le chemin du dernier document traité.


**Returns:**
java.lang.String - Le chemin du dernier document traité.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Obtient le statut du dernier document traité.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

