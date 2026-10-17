---
title: "TextOptions"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des options pour la récupération du texte du document à partir d'un index."
type: docs
weight: 41
url: /fr/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Fournit des options pour la récupération du texte du document à partir d'un index.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | Initialise une nouvelle instance de la classe  TextOptions . |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | Initialise une nouvelle instance de la classe  TextOptions . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Obtient l'extracteur de texte personnalisé qui a été utilisé pour l'indexation. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Définit l'extracteur de texte personnalisé qui a été utilisé pour l'indexation. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Obtient les champs de document supplémentaires qui ont été utilisés pour l'indexation. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Définit les champs de document supplémentaires qui ont été utilisés pour l'indexation. |
|
|  | [getCancellation()](#getCancellation--) | Obtient l'objet d'annulation. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Définit l'objet d'annulation. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Obtient une valeur indiquant si la balise Head est générée dans le HTML de sortie. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Définit une valeur indiquant si la balise Head est générée dans le HTML de sortie. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Initialise une nouvelle instance de la classe  TextOptions .


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


Initialise une nouvelle instance de la classe  TextOptions .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | données | java.lang.Object | Les données sérialisées. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Obtient l'extracteur de texte personnalisé qui a été utilisé pour l'indexation. La valeur par défaut est null. Notez que cette valeur n'est utilisée que si le texte du document n'a pas été enregistré dans l'index.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Définit l'extracteur de texte personnalisé qui a été utilisé pour l'indexation. La valeur par défaut est null. Notez que cette valeur n'est utilisée que si le texte du document n'a pas été enregistré dans l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'extracteur de texte personnalisé qui a été utilisé pour l'indexation. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Obtient les champs de document supplémentaires qui ont été utilisés pour l'indexation. La valeur par défaut est null. Notez que cette valeur n'est utilisée que si le texte du document n'a pas été enregistré dans l'index.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Les champs de document supplémentaires qui ont été utilisés pour l'indexation.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Définit les champs de document supplémentaires qui ont été utilisés pour l'indexation. La valeur par défaut est null. Notez que cette valeur n'est utilisée que si le texte du document n'a pas été enregistré dans l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Les champs de document supplémentaires qui ont été utilisés pour l'indexation. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Obtient l'objet d'annulation. La valeur par défaut est null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Définit l'objet d'annulation. La valeur par défaut est null.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'objet d'annulation. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Obtient une valeur indiquant si la balise Head est générée dans le HTML de sortie. La valeur par défaut est true.


**Returns:**
boolean - Une valeur indiquant si la balise Head est générée dans le HTML de sortie.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Définit une valeur indiquant si la balise Head est générée dans le HTML de sortie. La valeur par défaut est true.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si la balise Head est générée dans le HTML de sortie. |
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
