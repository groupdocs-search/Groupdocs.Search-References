---
title: "ExtractionOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour l'extraction de données à partir de documents."
type: docs
weight: 18
url: /fr/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Fournit des options pour l'extraction de données à partir de documents.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | Initialise une nouvelle instance de la classe  ExtractionOptions  . |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Initialise une nouvelle instance de la classe  ExtractionOptions  . |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Initialise une nouvelle instance de la classe  ExtractionOptions  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Obtient l'extracteur de texte personnalisé. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Définit ou définit l'extracteur de texte personnalisé. |
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
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Initialise une nouvelle instance de la classe  ExtractionOptions  .


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Initialise une nouvelle instance de la classe  ExtractionOptions  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | données | java.lang.Object | Les données sérialisées. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Initialise une nouvelle instance de la classe  ExtractionOptions  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Les options. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'extracteur personnalisé. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Le connecteur ocr. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Obtient l'extracteur de texte personnalisé. La valeur par défaut est  null .


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Définit ou définit l'extracteur de texte personnalisé. La valeur par défaut est  null .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'extracteur de texte personnalisé. |
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
