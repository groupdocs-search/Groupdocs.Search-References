---
title: "DocumentImage"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les données d'image d'un document."
type: docs
weight: 16
url: /fr/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Représente les données d'image d'un document.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Obtient le numéro ordinal de l'image dans le document. |
|
|  | [getFields()](#getFields--) | Obtient les champs extraits. |
|
|  | [getFrames()](#getFrames--) | Obtient les cadres d'image. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Obtient le numéro ordinal de l'image dans le document.


**Returns:**
int - Le numéro ordinal de l'image dans le document.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Obtient les champs extraits.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Les champs extraits.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Obtient les cadres d'image.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Les cadres d'image.

