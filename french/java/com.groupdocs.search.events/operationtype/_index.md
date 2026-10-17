---
title: "OperationType"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un type d'opération d'index."
type: docs
weight: 23
url: /fr/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Représente un type d'opération d'index.

## Fields

| Field | Description |
| --- | --- |
|  | [Indexing](#Indexing) | Ajout de documents à un index. |
|
|  | [Updating](#Updating) | Mise à jour de documents dans un index. |
|
|  | [Merging](#Merging) | Fusion d'index. |
|
|  | [Optimizing](#Optimizing) | Optimisation d'un index. |
|
|  | [Deleting](#Deleting) | Suppression de chemins d'un index. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Ajout de documents à un index.


### Updating {#Updating}
```
public static final OperationType Updating
```


Mise à jour de documents dans un index.


### Merging {#Merging}
```
public static final OperationType Merging
```


Fusion d'index.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Optimisation d'un index.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Suppression de chemins d'un index.


### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
