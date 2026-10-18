---
title: "TextOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per il recupero del testo del documento da un indice."
type: docs
weight: 41
url: /it/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Fornisce opzioni per il recupero del testo del documento da un indice.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | Inizializza una nuova istanza della classe  TextOptions . |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | Inizializza una nuova istanza della classe  TextOptions . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Ottiene l'estrattore di testo personalizzato utilizzato per l'indicizzazione. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Imposta l'estrattore di testo personalizzato utilizzato per l'indicizzazione. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Ottiene i campi documento aggiuntivi utilizzati per l'indicizzazione. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Imposta i campi documento aggiuntivi utilizzati per l'indicizzazione. |
|
|  | [getCancellation()](#getCancellation--) | Ottiene l'oggetto di cancellazione. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Imposta l'oggetto di cancellazione. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Ottiene un valore che indica se il tag Head viene generato nell'HTML di output. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Imposta un valore che indica se il tag Head viene generato nell'HTML di output. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Inizializza una nuova istanza della classe  TextOptions .


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


Inizializza una nuova istanza della classe  TextOptions .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | java.lang.Object | I dati serializzati. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Ottiene l'estrattore di testo personalizzato utilizzato per l'indicizzazione. Il valore predefinito è null. Nota che questo valore viene usato solo se il testo del documento non è stato salvato nell'indice.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Imposta l'estrattore di testo personalizzato utilizzato per l'indicizzazione. Il valore predefinito è null. Nota che questo valore viene usato solo se il testo del documento non è stato salvato nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'estrattore di testo personalizzato utilizzato per l'indicizzazione. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Ottiene i campi documento aggiuntivi utilizzati per l'indicizzazione. Il valore predefinito è null. Nota che questo valore viene usato solo se il testo del documento non è stato salvato nell'indice.


**Returns:**
com.groupdocs.search.common.DocumentField[] - I campi documento aggiuntivi utilizzati per l'indicizzazione.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Imposta i campi documento aggiuntivi utilizzati per l'indicizzazione. Il valore predefinito è null. Nota che questo valore viene usato solo se il testo del documento non è stato salvato nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | I campi documento aggiuntivi utilizzati per l'indicizzazione. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Ottiene l'oggetto di cancellazione. Il valore predefinito è null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Imposta l'oggetto di cancellazione. Il valore predefinito è null.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'oggetto di cancellazione. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Ottiene un valore che indica se il tag Head viene generato nell'HTML di output. Il valore predefinito è true.


**Returns:**
boolean - Un valore che indica se il tag Head viene generato nell'HTML di output.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Imposta un valore che indica se il tag Head viene generato nell'HTML di output. Il valore predefinito è true.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se il tag Head viene generato nell'HTML di output. |
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
