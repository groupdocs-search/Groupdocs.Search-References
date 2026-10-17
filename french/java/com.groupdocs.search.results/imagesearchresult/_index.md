---
title: "ImageSearchResult"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente le résultat d'une recherche d'image inversée."
type: docs
weight: 17
url: /fr/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Représente le résultat d'une recherche d'image inversée.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Obtient le nombre d'images trouvées. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Obtient l'image trouvée par indice. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Obtient le nombre d'images trouvées.


**Returns:**
int - Le nombre d'images trouvées.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Obtient l'image trouvée par indice.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | index | int | L'indice d'une image trouvée. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

