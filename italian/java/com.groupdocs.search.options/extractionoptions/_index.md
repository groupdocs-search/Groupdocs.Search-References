---
title: "ExtractionOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per l'estrazione dei dati dai documenti."
type: docs
weight: 18
url: /it/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Fornisce opzioni per l'estrazione dei dati dai documenti.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | Inizializza una nuova istanza della classe ExtractionOptions. |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Inizializza una nuova istanza della classe ExtractionOptions. |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Inizializza una nuova istanza della classe ExtractionOptions. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Ottiene l'estrattore di testo personalizzato. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Imposta o imposta l'estrattore di testo personalizzato. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Restituisce un valore che indica se rilevare automaticamente la codifica o meno. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Imposta un valore che indica se rilevare automaticamente la codifica o meno. |
|
|  | [getEncoding()](#getEncoding--) | Restituisce la codifica utilizzata per estrarre il testo dai documenti di testo. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Imposta la codifica utilizzata per estrarre il testo dai documenti di testo. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Ottiene un valore che indica se la modalità raw è utilizzata per l'estrazione del testo, se possibile. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Imposta un valore che indica se la modalità raw è utilizzata per l'estrazione del testo, se possibile. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Ottiene le opzioni per l'indicizzazione dei campi di metadati. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Ottiene le opzioni per l'elaborazione OCR e l'indicizzazione del testo riconosciuto. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Ottiene le opzioni di indicizzazione delle immagini per la ricerca inversa di immagini. |
|
| [getCore()](#getCore--) |  |
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Inizializza una nuova istanza della classe ExtractionOptions.


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Inizializza una nuova istanza della classe ExtractionOptions.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | java.lang.Object | I dati serializzati. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Inizializza una nuova istanza della classe ExtractionOptions.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Le opzioni. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'estrattore personalizzato. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Il connettore ocr. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Ottiene l'estrattore di testo personalizzato. Il valore predefinito è  null .


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Imposta o imposta l'estrattore di testo personalizzato. Il valore predefinito è  null .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'estrattore di testo personalizzato. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Ottiene un valore che indica se rilevare automaticamente la codifica o meno. Il valore predefinito è  false .


**Returns:**
boolean - Un valore che indica se rilevare automaticamente la codifica o meno.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Imposta un valore che indica se rilevare automaticamente la codifica o meno. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se rilevare automaticamente la codifica o meno. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Ottiene la codifica utilizzata per estrarre il testo dai documenti di testo. Il valore predefinito è  null , il che significa che viene utilizzata la codifica predefinita UTF-8. Se AutoDetectEncoding è  true  allora questo valore è usato come codifica predefinita.


**Returns:**
java.lang.String - La codifica utilizzata per estrarre il testo dai documenti di testo.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Imposta la codifica utilizzata per estrarre il testo dai documenti di testo. Il valore predefinito è  null , il che significa che viene utilizzata la codifica predefinita UTF-8. Se AutoDetectEncoding è  true  allora questo valore è usato come codifica predefinita.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | La codifica utilizzata per estrarre il testo dai documenti di testo. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Restituisce un valore che indica se la modalità raw è utilizzata per l'estrazione del testo, se possibile. Il valore predefinito è true. La modalità raw può aumentare significativamente la velocità di indicizzazione, ma la modalità normale migliora la formattazione del testo estratto.


**Returns:**
boolean - Un valore che indica se la modalità raw è utilizzata per l'estrazione del testo, se possibile.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Imposta un valore che indica se la modalità raw è utilizzata per l'estrazione del testo, se possibile. Il valore predefinito è true. La modalità raw può aumentare significativamente la velocità di indicizzazione, ma la modalità normale migliora la formattazione del testo estratto.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se la modalità raw è utilizzata per l'estrazione del testo, se possibile. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Ottiene le opzioni per l'indicizzazione dei campi di metadati.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Ottiene le opzioni per l'elaborazione OCR e l'indicizzazione del testo riconosciuto.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Ottiene le opzioni di indicizzazione delle immagini per la ricerca inversa di immagini.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
