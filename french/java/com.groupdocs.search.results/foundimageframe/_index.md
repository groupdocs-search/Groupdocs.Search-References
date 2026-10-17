---
title: "FoundImageFrame"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente une trame d'image trouvée."
type: docs
weight: 16
url: /fr/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Représente une trame d'image trouvée.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Obtient les informations du document. |
|
|  | [getImageIndex()](#getImageIndex--) | Obtient le numéro ordinal de l'image dans le document. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Obtient l'index de la trame dans l'image. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Obtient le nombre de bits non correspondants dans le hachage de l'image. |
|
|  | [toString()](#toString--) | Renvoie un  System.String  qui représente le  FoundImageFrame  actuel. |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Obtient les informations du document.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Obtient le numéro ordinal de l'image dans le document.


**Returns:**
int - Le numéro ordinal de l'image dans le document.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Obtient l'index de la trame dans l'image.


**Returns:**
int - L'index de la trame dans l'image.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Obtient le nombre de bits non correspondants dans le hachage de l'image.


**Returns:**
int - Le nombre de bits non correspondants dans le hachage de l'image.

### toString() {#toString--}
```
public abstract String toString()
```


Renvoie un  System.String  qui représente le  FoundImageFrame  actuel.


**Returns:**
java.lang.String - Un  System.String  qui représente le  FoundImageFrame  actuel.

