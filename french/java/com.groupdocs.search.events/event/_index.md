---
title: "Événement"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Cette classe est destinée à être héritée lors de l'abonnement aux événements."
type: docs
weight: 11
url: /fr/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Cette classe est destinée à être héritée lors de l'abonnement aux événements.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [Event()](#Event--) | Initialise une nouvelle instance de la classe  Event  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Ajoute un écouteur pour l'événement. |
|
|  | [remove(T delegate)](#remove-T-) | Supprime un écouteur pour l'événement. |
|
|  | [isEmpty()](#isEmpty--) | Vérifie la présence d'au moins un écouteur. |
|
### Event() {#Event--}
```
public Event()
```


Initialise une nouvelle instance de la classe  Event  .


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Ajoute un écouteur pour l'événement.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | delegate | T | Un écouteur pour l'événement à ajouter. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Supprime un écouteur pour l'événement.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | delegate | T | Un écouteur pour l'événement à supprimer. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Vérifie la présence d'au moins un écouteur.


**Returns:**
boolean - Une valeur indiquant qu'au moins un écouteur a été ajouté pour l'événement.

