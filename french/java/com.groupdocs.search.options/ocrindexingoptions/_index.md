---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour le traitement OCR et l'indexation du texte reconnu."
type: docs
weight: 31
url: /fr/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Fournit des options pour le traitement OCR et l'indexation du texte reconnu.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Obtient une valeur indiquant s'il faut reconnaître le texte dans des fichiers image séparés. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Définit une valeur indiquant s'il faut reconnaître le texte dans des fichiers image séparés. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Obtient une valeur indiquant s'il faut reconnaître le texte dans des images qui sont des éléments d'un conteneur (par exemple, des images dans une archive ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Définit une valeur indiquant s'il faut reconnaître le texte dans des images qui sont des éléments d'un conteneur (par exemple, des images dans une archive ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Obtient une valeur indiquant s'il faut reconnaître le texte dans des images intégrées (par exemple, des images dans un document DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Définit une valeur indiquant s'il faut reconnaître le texte dans des images intégrées (par exemple, des images dans un document DOCX). |
|
|  | [getOcrConnector()](#getOcrConnector--) | Obtient un connecteur OCR utilisé pour le traitement OCR. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Définit un connecteur OCR utilisé pour le traitement OCR. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Obtient une valeur indiquant s'il faut reconnaître le texte dans des fichiers image séparés. La valeur par défaut est  false .


**Returns:**
boolean - Une valeur indiquant s'il faut reconnaître le texte dans des fichiers image séparés.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Définit une valeur indiquant s'il faut reconnaître le texte dans des fichiers image séparés. La valeur par défaut est  false .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s'il faut reconnaître le texte dans des fichiers image séparés. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Obtient une valeur indiquant s'il faut reconnaître le texte dans des images qui sont des éléments d'un conteneur (par exemple, des images dans une archive ZIP). La valeur par défaut est  false .


**Returns:**
boolean - Une valeur indiquant s'il faut reconnaître le texte dans des images qui sont des éléments d'un conteneur.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Définit une valeur indiquant s'il faut reconnaître le texte dans des images qui sont des éléments d'un conteneur (par exemple, des images dans une archive ZIP). La valeur par défaut est  false .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s'il faut reconnaître le texte dans des images qui sont des éléments d'un conteneur. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Obtient une valeur indiquant s'il faut reconnaître le texte dans des images intégrées (par exemple, des images dans un document DOCX). La valeur par défaut est  false .


**Returns:**
boolean - Une valeur indiquant s'il faut reconnaître le texte dans des images intégrées.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Définit une valeur indiquant s'il faut reconnaître le texte dans des images intégrées (par exemple, des images dans un document DOCX). La valeur par défaut est  false .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s'il faut reconnaître le texte dans des images intégrées. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Obtient un connecteur OCR utilisé pour le traitement OCR. La valeur par défaut est  null , ce qui signifie qu'aucun OCR n'est utilisé.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Définit un connecteur OCR utilisé pour le traitement OCR. La valeur par défaut est  null , ce qui signifie qu'aucun OCR n'est utilisé.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Un connecteur OCR qui est utilisé pour le traitement OCR. |
|

