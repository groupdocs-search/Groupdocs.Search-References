---
title: "IndexingOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour l'opération d'indexation."
type: docs
weight: 25
url: /fr/java/com.groupdocs.search.options/indexingoptions/
---
**Inheritance:**
java.lang.Object
```
public class IndexingOptions
```

Fournit des options pour l'opération d'indexation.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [IndexingOptions()](#IndexingOptions--) | Initialise une nouvelle instance de la classe  IndexingOptions . |
|
|  | [IndexingOptions(Object data)](#IndexingOptions-java.lang.Object-) | Initialise une nouvelle instance de la classe  IndexingOptions . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getThreads()](#getThreads--) | Obtient le nombre de threads utilisés pour l'indexation. |
|
|  | [setThreads(int value)](#setThreads-int-) | Définit le nombre de threads utilisés pour l'indexation. |
|
|  | [isAsync()](#isAsync--) | Obtient le drapeau d'exécution asynchrone de l'opération. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Définit le drapeau d'exécution asynchrone de l'opération. |
|
|  | [getCancellation()](#getCancellation--) | Obtient l'objet d'annulation de l'opération. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Définit l'objet d'annulation de l'opération. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Obtient une valeur indiquant s'il faut détecter l'encodage automatiquement ou non. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Définit une valeur indiquant s'il faut détecter l'encodage automatiquement ou non. |
|
|  | [getEncoding()](#getEncoding--) | Obtient l'encodage utilisé pour extraire le texte des documents texte. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Définit le codage utilisé pour extraire le texte des documents texte. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Obtient une valeur indiquant si le mode brut est utilisé pour l'extraction de texte si possible. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Définit une valeur indiquant si le mode brut est utilisé pour l'extraction de texte si possible. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Obtient les options pour l'indexation des champs de métadonnées. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Obtient les options pour le traitement OCR et l'indexation du texte reconnu. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Obtient les options d'indexation d'images pour la recherche d'images inversée. |
|
| [getCore()](#getCore--) |  |
### IndexingOptions() {#IndexingOptions--}
```
public IndexingOptions()
```


Initialise une nouvelle instance de la classe  IndexingOptions .


### IndexingOptions(Object data) {#IndexingOptions-java.lang.Object-}
```
public IndexingOptions(Object data)
```


Initialise une nouvelle instance de la classe  IndexingOptions .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | données | java.lang.Object | Les données sérialisées. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Obtient le nombre de threads utilisés pour l'indexation. La valeur par défaut est 1.


**Returns:**
int - Le nombre de threads utilisés pour l'indexation.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Définit le nombre de threads utilisés pour l'indexation. La valeur par défaut est 1.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre de threads utilisés pour l'indexation. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Obtient le drapeau d'exécution asynchrone de l'opération. La valeur par défaut est false.


**Returns:**
boolean - Le drapeau d'exécution asynchrone de l'opération.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Définit le drapeau d'exécution asynchrone de l'opération. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Le drapeau d'exécution asynchrone de l'opération. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Obtient l'objet d'annulation de l'opération. La valeur par défaut est null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Définit l'objet d'annulation de l'opération. La valeur par défaut est null.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'objet d'annulation de l'opération. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Obtient une valeur indiquant s'il faut détecter le codage automatiquement ou non. La valeur par défaut est false.


**Returns:**
boolean - Une valeur indiquant s'il faut détecter le codage automatiquement ou non.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Définit une valeur indiquant s'il faut détecter le codage automatiquement ou non. La valeur par défaut est false.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant s'il faut détecter le codage automatiquement ou non. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Obtient le codage utilisé pour extraire le texte des documents texte. La valeur par défaut est null, ce qui signifie que le codage par défaut UTF-8 est utilisé. Si AutoDetectEncoding est true, alors cette valeur est utilisée comme codage par défaut.


**Returns:**
java.lang.String - Le codage utilisé pour extraire le texte des documents texte.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Définit le codage utilisé pour extraire le texte des documents texte. La valeur par défaut est null, ce qui signifie que le codage par défaut UTF-8 est utilisé. Si AutoDetectEncoding est true, alors cette valeur est utilisée comme codage par défaut.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Le codage utilisé pour extraire le texte des documents texte. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Obtient une valeur indiquant si le mode brut est utilisé pour l'extraction de texte si possible. La valeur par défaut est true. Le mode brut peut augmenter considérablement la vitesse d'indexation, mais le mode normal améliore le formatage du texte extrait.


**Returns:**
booléen - Une valeur indiquant si le mode brut est utilisé pour l'extraction de texte si possible.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Définit une valeur indiquant si le mode brut est utilisé pour l'extraction de texte si possible. La valeur par défaut est true. Le mode brut peut augmenter considérablement la vitesse d'indexation, mais le mode normal améliore le formatage du texte extrait.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si le mode brut est utilisé pour l'extraction de texte si possible. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Obtient les options pour l'indexation des champs de métadonnées.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Obtient les options pour le traitement OCR et l'indexation du texte reconnu.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Obtient les options d'indexation d'images pour la recherche d'images inversée.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
