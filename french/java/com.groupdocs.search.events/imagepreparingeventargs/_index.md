---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement de démarrage de la préparation d'une image."
type: docs
weight: 15
url: /fr/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Représente les arguments de l'événement de démarrage de la préparation d'une image.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Obtient la clé du document. |
|
|  | [getInnerPath()](#getInnerPath--) | Obtient le chemin interne d'un document imbriqué. |
|
|  | [getImageIndex()](#getImageIndex--) | Obtient le numéro ordinal de l'image dans le document. |
|
|  | [getImageFrames()](#getImageFrames--) | Obtient les cadres d'image. |
|
|  | [getImageStream()](#getImageStream--) | Obtient le flux d'image. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Obtient la clé du document.


**Returns:**
java.lang.String - La clé du document.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Obtient le chemin interne d'un document imbriqué.


**Returns:**
java.lang.String[] - Le chemin interne d'un document imbriqué.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Obtient le numéro ordinal de l'image dans le document.


**Returns:**
int - Le numéro ordinal de l'image dans le document.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Obtient les cadres d'image.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Les cadres d'image.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Obtient le flux d'image.


**Returns:**
java.io.InputStream - Le flux d'image.

