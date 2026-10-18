---
title: "IndexingOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per l'operazione di indicizzazione."
type: docs
weight: 25
url: /it/java/com.groupdocs.search.options/indexingoptions/
---
**Inheritance:**
java.lang.Object
```
public class IndexingOptions
```

Fornisce opzioni per l'operazione di indicizzazione.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [IndexingOptions()](#IndexingOptions--) | Inizializza una nuova istanza della classe IndexingOptions. |
|
|  | [IndexingOptions(Object data)](#IndexingOptions-java.lang.Object-) | Inizializza una nuova istanza della classe IndexingOptions. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getThreads()](#getThreads--) | Restituisce il numero di thread utilizzati per l'indicizzazione. |
|
|  | [setThreads(int value)](#setThreads-int-) | Imposta il numero di thread utilizzati per l'indicizzazione. |
|
|  | [isAsync()](#isAsync--) | Restituisce il flag dell'esecuzione asincrona dell'operazione. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Imposta il flag dell'esecuzione asincrona dell'operazione. |
|
|  | [getCancellation()](#getCancellation--) | Restituisce l'oggetto di annullamento dell'operazione. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Imposta l'oggetto di annullamento dell'operazione. |
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
### IndexingOptions() {#IndexingOptions--}
```
public IndexingOptions()
```


Inizializza una nuova istanza della classe IndexingOptions.


### IndexingOptions(Object data) {#IndexingOptions-java.lang.Object-}
```
public IndexingOptions(Object data)
```


Inizializza una nuova istanza della classe IndexingOptions.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | java.lang.Object | I dati serializzati. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Ottiene il numero di thread utilizzati per l'indicizzazione. Il valore predefinito è  1 .


**Returns:**
int - Il numero di thread utilizzati per l'indicizzazione.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Imposta il numero di thread utilizzati per l'indicizzazione. Il valore predefinito è  1 .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero di thread utilizzati per l'indicizzazione. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Ottiene il flag dell'esecuzione asincrona dell'operazione. Il valore predefinito è  false .


**Returns:**
boolean - Il flag dell'esecuzione asincrona dell'operazione.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Imposta il flag dell'esecuzione asincrona dell'operazione. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il flag dell'esecuzione asincrona dell'operazione. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Ottiene l'oggetto di annullamento dell'operazione. Il valore predefinito è  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Imposta l'oggetto di annullamento dell'operazione. Il valore predefinito è  null .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'oggetto di annullamento dell'operazione. |
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
