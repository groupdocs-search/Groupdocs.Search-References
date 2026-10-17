---
title: "DocumentIndexedEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement de fin d'indexation d'un document."
type: docs
weight: 12
url: /fr/java/com.groupdocs.search.scaling.events/documentindexedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentIndexedEventArgs extends EventArgs
```

Représente les arguments de l'événement de fin d'indexation d'un document.

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Obtient l'index de la partition. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Obtient la clé du document. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Obtient l'index de la partition.


**Returns:**
int - L'index de la partition.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Obtient la clé du document.


**Returns:**
java.lang.String - La clé du document.

