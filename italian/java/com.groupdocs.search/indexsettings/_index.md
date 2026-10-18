---
title: "IndexSettings"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta le impostazioni dell'indice che consentono di personalizzare le operazioni di indicizzazione."
type: docs
weight: 19
url: /it/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Rappresenta le impostazioni dell'indice che consentono di personalizzare le operazioni di indicizzazione.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Impostazione del tipo di indice
Index index = new Index(indexFolder, settings); // Creazione di un indice
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | Inizializza una nuova istanza della classe  IndexSettings . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Restituisce un valore che indica se l'indice è memorizzato in memoria o su disco. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Restituisce un valore che indica se utilizzare le parole di stop o meno. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Imposta un valore che indica se utilizzare le parole di stop o meno. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Restituisce il numero massimo di report di indicizzazione. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Imposta il numero massimo di report di indicizzazione. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Restituisce il numero massimo di report di ricerca. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Imposta il numero massimo di report di ricerca. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Restituisce un valore che indica se utilizzare le sostituzioni di caratteri o meno. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Imposta un valore che indica se utilizzare le sostituzioni di caratteri o meno. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Restituisce un filtro di documento. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Imposta un filtro di documento. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Restituisce le impostazioni di archiviazione del testo. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Imposta le impostazioni di archiviazione del testo. |
|
|  | [getIndexType()](#getIndexType--) | Restituisce il tipo di indice. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Imposta il tipo di indice. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Ottiene il numero di thread utilizzati per la ricerca. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Imposta il numero di thread utilizzati per la ricerca. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Ottiene la raccolta di estrattori personalizzati. |
|
|  | [getLogger()](#getLogger--) | Ottiene un logger utilizzato per registrare eventi ed errori nell'indice. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Imposta un logger utilizzato per registrare eventi ed errori nell'indice. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Inizializza una nuova istanza della classe  IndexSettings .


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Restituisce un valore che indica se l'indice è memorizzato in memoria o su disco.


**Returns:**
boolean - Un valore che indica se l'indice è memorizzato in memoria o su disco.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Ottiene un valore che indica se utilizzare le parole di stop o meno. Il valore predefinito è  true .


**Returns:**
boolean - Un valore che indica se utilizzare le parole di stop o meno.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Imposta un valore che indica se utilizzare le parole di stop o meno. Il valore predefinito è  true .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se utilizzare le parole di stop o meno. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Ottiene il numero massimo di report di indicizzazione. Il valore predefinito è  5 .


**Returns:**
int - Il numero massimo di report di indicizzazione.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Imposta il numero massimo di report di indicizzazione. Il valore predefinito è  5 .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di report di indicizzazione. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Ottiene il numero massimo di report di ricerca. Il valore predefinito è  10 .


**Returns:**
int - Il numero massimo di report di ricerca.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Imposta il numero massimo di report di ricerca. Il valore predefinito è  10 .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di report di ricerca. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Ottiene un valore che indica se utilizzare le sostituzioni di caratteri o meno. Il valore predefinito è  false .


**Returns:**
boolean - Un valore che indica se utilizzare le sostituzioni di caratteri o meno.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Imposta un valore che indica se utilizzare le sostituzioni di caratteri o meno. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se utilizzare le sostituzioni di caratteri o meno. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Ottiene un filtro documento. Il  DocumentFilter  funziona sulla logica di inclusione. Utilizzare la classe  DocumentFilter  per creare un'istanza di filtro documento. Il valore predefinito è  null , il che significa che tutti i documenti aggiunti sono indicizzati.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

L'esempio dimostra come impostare il filtro documento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un filtro che salta i documenti con estensioni '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creazione del filtro per estensione file
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Inversione del filtro per estensione file
settings.setDocumentFilter(invertedFilter);
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder, settings);
// Indicizzazione dei documenti
index.add(documentsFolder);
// Ricerca
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Imposta un filtro per i documenti. Il  DocumentFilter  funziona sulla logica di inclusione. Utilizza la classe  GroupDocs.Search.Options.DocumentFilter  per creare istanze di un filtro per i documenti. Il valore predefinito è  null , il che significa che tutti i documenti aggiunti vengono indicizzati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Il filtro per i documenti. |

L'esempio dimostra come impostare il filtro documento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un filtro che salta i documenti con estensioni '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creazione del filtro per estensione file
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Inversione del filtro per estensione file
settings.setDocumentFilter(invertedFilter);
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder, settings);
// Indicizzazione dei documenti
index.add(documentsFolder);
// Ricerca
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Ottiene le impostazioni di archiviazione del testo. Il valore predefinito è  null , il che significa che i testi dei documenti non vengono memorizzati.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

L'esempio dimostra come impostare le impostazioni di archiviazione del testo.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione dell'istanza delle impostazioni dell'indice
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Impostazione di un livello di compressione elevato per l'archiviazione del testo dell'indice
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder, settings);
// Indicizzazione dei documenti
index.add(documentsFolder);
// Ricerca
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Imposta le impostazioni di archiviazione del testo. Il valore predefinito è  null , il che significa che i testi dei documenti non vengono memorizzati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | Le impostazioni di archiviazione del testo. |

L'esempio dimostra come impostare le impostazioni di archiviazione del testo.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione dell'istanza delle impostazioni dell'indice
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Impostazione di un livello di compressione elevato per l'archiviazione del testo dell'indice
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder, settings);
// Indicizzazione dei documenti
index.add(documentsFolder);
// Ricerca
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Ottiene il tipo di indice. Il valore predefinito è  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Imposta il tipo di indice. Il valore predefinito è  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Il tipo di indice. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Ottiene il numero di thread utilizzati per la ricerca. Il valore predefinito è  GroupDocs.Search.Options.NumberOfThreads.Default , il che significa che la ricerca verrà eseguita utilizzando un numero di thread pari al numero di core del processore.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Imposta il numero di thread utilizzati per la ricerca. Il valore predefinito è  GroupDocs.Search.Options.NumberOfThreads.Default , il che significa che la ricerca verrà eseguita utilizzando un numero di thread pari al numero di core del processore.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Il numero di thread utilizzati per la ricerca. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Ottiene la collezione di estrattori personalizzati. L'esempio completo di implementazione di un estrattore personalizzato è presentato nella documentazione dell'interfaccia  GroupDocs.Search.Common.IFieldExtractor .


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Ottiene un logger utilizzato per registrare eventi ed errori nell'indice. Nota che il logger non viene salvato e deve essere creato e assegnato ogni volta che l'indice viene creato o caricato.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Imposta un logger utilizzato per registrare eventi ed errori nell'indice. Nota che il logger non viene salvato e deve essere creato e assegnato ogni volta che l'indice viene creato o caricato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | Un logger utilizzato per registrare eventi ed errori nell'indice. |
|

