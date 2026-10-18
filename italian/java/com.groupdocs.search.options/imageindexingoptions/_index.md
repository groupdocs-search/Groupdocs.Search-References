---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni di indicizzazione delle immagini per la ricerca inversa di immagini."
type: docs
weight: 23
url: /it/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Fornisce opzioni di indicizzazione delle immagini per la ricerca inversa di immagini.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Ottiene un valore che indica se indicizzare file immagine separati. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Imposta un valore che indica se indicizzare file immagine separati. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Ottiene un valore che indica se indicizzare immagini che sono elementi in un contenitore (ad esempio, immagini in un archivio ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Imposta un valore che indica se indicizzare immagini che sono elementi in un contenitore (ad esempio, immagini in un archivio ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Ottiene un valore che indica se indicizzare immagini incorporate (ad esempio, immagini in un documento DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Imposta un valore che indica se indicizzare immagini incorporate (ad esempio, immagini in un documento DOCX). |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Ottiene un valore che indica se indicizzare file immagine separati. Il valore predefinito è  false .


**Returns:**
boolean - Un valore che indica se indicizzare file immagine separati.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Imposta un valore che indica se indicizzare file immagine separati. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se indicizzare file immagine separati. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Ottiene un valore che indica se indicizzare immagini che sono elementi in un contenitore (ad esempio, immagini in un archivio ZIP). Il valore predefinito è  false .


**Returns:**
boolean - Un valore che indica se indicizzare le immagini che sono elementi in un contenitore.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Imposta un valore che indica se indicizzare le immagini che sono elementi in un contenitore (ad esempio, immagini in un archivio ZIP). Il valore predefinito è false.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se indicizzare le immagini che sono elementi in un contenitore. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Ottiene un valore che indica se indicizzare le immagini incorporate (ad esempio, immagini in un documento DOCX). Il valore predefinito è false.


**Returns:**
boolean - Un valore che indica se indicizzare le immagini incorporate.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Imposta un valore che indica se indicizzare le immagini incorporate (ad esempio, immagini in un documento DOCX). Il valore predefinito è false.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se indicizzare le immagini incorporate. |
|

