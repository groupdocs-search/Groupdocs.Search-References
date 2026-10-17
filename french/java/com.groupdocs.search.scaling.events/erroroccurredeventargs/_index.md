---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement d'une erreur survenant dans l'un des nœuds du réseau de recherche."
type: docs
weight: 13
url: /fr/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Représente les arguments de l'événement d'une erreur survenant dans l'un des nœuds du réseau de recherche.

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Obtient l'index du nœud du réseau de recherche. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Obtient l'index du service du nœud du réseau de recherche. |
|
|  | [getMessage()](#getMessage--) | Obtient le message d'erreur. |
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

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Obtient le message d'erreur.


**Returns:**
java.lang.String - Le message d'erreur.

