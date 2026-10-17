---
title: "IndexInfo"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Contient des informations de base sur un index."
type: docs
weight: 24
url: /fr/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Contient des informations de base sur un index.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Obtient l'identifiant unique de l'index. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Obtient le nom complet du dossier où l'index est situé. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Obtient le statut de l'index. |
|
|  | [getVersion()](#getVersion--) | Obtient la version de l'index. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Obtient le nombre de segments d'index. |
|
|  | [getTermCount()](#getTermCount--) | Obtient le nombre de mots dans l'index. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Obtient l'identifiant unique de l'index.


**Returns:**
java.util.UUID - L'identifiant unique de l'index.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Obtient le nom complet du dossier où l'index est situé.


**Returns:**
java.lang.String - Le nom complet du dossier où l'index est situé.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Obtient le statut de l'index.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Obtient la version de l'index.


**Returns:**
java.lang.String - La version de l'index.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Obtient le nombre de segments d'index.


**Returns:**
int - Le nombre de segments d'index.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Obtient le nombre de mots dans l'index.


**Returns:**
int - Le nombre de mots dans l'index.

