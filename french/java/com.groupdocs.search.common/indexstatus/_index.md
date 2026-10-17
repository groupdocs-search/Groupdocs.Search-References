---
title: "IndexStatus"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Spécifie un statut d'index."
type: docs
weight: 41
url: /fr/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Spécifie un statut d'index.

## Fields

| Field | Description |
| --- | --- |
|  | [Ready](#Ready) | L'index est libre et prêt à être modifié. |
|
|  | [Failed](#Failed) | L'index doit être rechargé en raison d'une erreur. |
|
|  | [Indexing](#Indexing) | L'index effectue une opération d'indexation. |
|
|  | [Updating](#Updating) | L'index effectue une opération de mise à jour. |
|
|  | [Merging](#Merging) | L'index effectue une opération de fusion. |
|
|  | [Optimizing](#Optimizing) | L'index effectue une opération d'optimisation. |
|
|  | [Deleting](#Deleting) | L'index effectue une opération de suppression. |
|
|  | [Renaming](#Renaming) | L'index effectue une opération de renommage. |
|
|  | [ChangingAttributes](#ChangingAttributes) | L'index modifie les attributs. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


L'index est libre et prêt à être modifié.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


L'index doit être rechargé en raison d'une erreur.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


L'index effectue une opération d'indexation.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


L'index effectue une opération de mise à jour.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


L'index effectue une opération de fusion.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


L'index effectue une opération d'optimisation.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


L'index effectue une opération de suppression.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


L'index effectue une opération de renommage.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


L'index modifie les attributs.


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
