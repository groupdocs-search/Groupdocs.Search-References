---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options d'indexation d'images pour la recherche d'images inversée."
type: docs
weight: 23
url: /fr/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Fournit des options d'indexation d'images pour la recherche d'images inversée.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Obtient une valeur indiquant s'il faut indexer des fichiers image séparés. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Définit une valeur indiquant s'il faut indexer des fichiers image séparés. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Obtient une valeur indiquant s'il faut indexer les images qui sont des éléments d'un conteneur (par exemple, des images dans une archive ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Définit une valeur indiquant s'il faut indexer les images qui sont des éléments d'un conteneur (par exemple, des images dans une archive ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Obtient une valeur indiquant s'il faut indexer les images intégrées (par exemple, des images dans un document DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Définit une valeur indiquant s'il faut indexer les images intégrées (par exemple, des images dans un document DOCX). |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Obtient une valeur indiquant s'il faut indexer des fichiers image séparés. La valeur par défaut est  false .


**Returns:**
boolean - Une valeur indiquant s'il faut indexer des fichiers image séparés.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Définit une valeur indiquant s'il faut indexer des fichiers image séparés. La valeur par défaut est  false .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s'il faut indexer des fichiers image séparés. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Obtient une valeur indiquant s'il faut indexer les images qui sont des éléments d'un conteneur (par exemple, des images dans une archive ZIP). La valeur par défaut est  false .


**Returns:**
boolean - Une valeur indiquant s’il faut indexer les images qui sont des éléments d’un conteneur.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Définit une valeur indiquant s’il faut indexer les images qui sont des éléments d’un conteneur (par exemple, des images dans une archive ZIP). La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s’il faut indexer les images qui sont des éléments d’un conteneur. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Obtient une valeur indiquant s’il faut indexer les images intégrées (par exemple, des images dans un document DOCX). La valeur par défaut est false.


**Returns:**
boolean - Une valeur indiquant s’il faut indexer les images intégrées.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Définit une valeur indiquant s’il faut indexer les images intégrées (par exemple, des images dans un document DOCX). La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s’il faut indexer les images intégrées. |
|

