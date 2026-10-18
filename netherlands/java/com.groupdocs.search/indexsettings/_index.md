---
title: "IndexSettings"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de indexinstellingen voor die het mogelijk maken de indexeerbewerkingen aan te passen."
type: docs
weight: 19
url: /nl/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Stelt de indexinstellingen voor die het mogelijk maken de indexeerbewerkingen aan te passen.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Instellen van het indextype
Index index = new Index(indexFolder, settings); // Een index maken
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | Initialiseert een nieuw exemplaar van de  IndexSettings  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Haalt een waarde op die aangeeft of de index in het geheugen of op schijf is opgeslagen. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Haalt een waarde op die aangeeft of stopwoorden al dan niet worden gebruikt. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Stelt een waarde in die aangeeft of stopwoorden al dan niet worden gebruikt. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Haalt het maximale aantal indexeringsrapporten op. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Stelt het maximale aantal indexeringsrapporten in. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Haalt het maximale aantal zoekrapporten op. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Stelt het maximale aantal zoekrapporten in. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Haalt een waarde op die aangeeft of tekenvervangingen al dan niet worden gebruikt. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Stelt een waarde in die aangeeft of tekenvervangingen al dan niet worden gebruikt. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Haalt een documentfilter op. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Stelt een documentfilter in. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Haalt de tekstopslaginstellingen op. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Stelt de tekstopslaginstellingen in. |
|
|  | [getIndexType()](#getIndexType--) | Haalt het indextype op. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Stelt het indextype in. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Haalt het aantal threads op dat wordt gebruikt voor de zoekopdracht. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Stelt het aantal threads in dat wordt gebruikt voor de zoekopdracht. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Haalt de aangepaste extractorcollectie op. |
|
|  | [getLogger()](#getLogger--) | Haalt een logger op die wordt gebruikt voor het loggen van gebeurtenissen en fouten in de index. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Stelt een logger in die wordt gebruikt voor het loggen van gebeurtenissen en fouten in de index. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Initialiseert een nieuw exemplaar van de  IndexSettings  klasse.


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Haalt een waarde op die aangeeft of de index in het geheugen of op schijf is opgeslagen.


**Returns:**
boolean - Een waarde die aangeeft of de index in het geheugen of op schijf wordt opgeslagen.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Haalt een waarde op die aangeeft of stopwoorden al dan niet worden gebruikt. De standaardwaarde is  true .


**Returns:**
boolean - Een waarde die aangeeft of stopwoorden al dan niet worden gebruikt.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Stelt een waarde in die aangeeft of stopwoorden al dan niet worden gebruikt. De standaardwaarde is  true .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of stopwoorden al dan niet worden gebruikt. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Haalt het maximale aantal indexeringsrapporten op. De standaardwaarde is  5 .


**Returns:**
int - Het maximale aantal indexeringsrapporten.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Stelt het maximale aantal indexeringsrapporten in. De standaardwaarde is  5 .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal indexeringsrapporten. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Haalt het maximale aantal zoekrapporten op. De standaardwaarde is  10 .


**Returns:**
int - Het maximale aantal zoekrapporten.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Stelt het maximale aantal zoekrapporten in. De standaardwaarde is  10 .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal zoekrapporten. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Haalt een waarde op die aangeeft of tekenvervangingen al dan niet worden gebruikt. De standaardwaarde is  false .


**Returns:**
boolean - Een waarde die aangeeft of tekenvervangingen al dan niet worden gebruikt.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Stelt een waarde in die aangeeft of tekenvervangingen al dan niet worden gebruikt. De standaardwaarde is  false .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of tekenvervangingen al dan niet worden gebruikt. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Haalt een documentfilter op. De  DocumentFilter  werkt volgens de inclusielogica. Gebruik de  DocumentFilter  klasse om een documentfilter‑instantie te maken. De standaardwaarde is  null , wat betekent dat alle toegevoegde documenten worden geïndexeerd.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

Het voorbeeld toont hoe het documentfilter in te stellen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een filter maken dat documenten met extensies '.doc', '.docx', '.rtf' overslaat
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Een filter voor bestandsextensies maken
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Filter voor bestandsextensies omkeren
settings.setDocumentFilter(invertedFilter);
// Een index maken in de opgegeven map
Index index = new Index(indexFolder, settings);
// Documenten indexeren
index.add(documentsFolder);
// Zoeken
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Stelt een documentfilter in. De  DocumentFilter  werkt volgens de inclusielogica. Gebruik de  GroupDocs.Search.Options.DocumentFilter  klasse voor het maken van documentfilter-instanties. De standaardwaarde is  null , wat betekent dat alle toegevoegde documenten worden geïndexeerd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Het documentfilter. |

Het voorbeeld toont hoe het documentfilter in te stellen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een filter maken dat documenten met extensies '.doc', '.docx', '.rtf' overslaat
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Een filter voor bestandsextensies maken
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Filter voor bestandsextensies omkeren
settings.setDocumentFilter(invertedFilter);
// Een index maken in de opgegeven map
Index index = new Index(indexFolder, settings);
// Documenten indexeren
index.add(documentsFolder);
// Zoeken
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Haalt de instellingen voor tekstopslag op. De standaardwaarde is  null , wat betekent dat documentteksten niet worden opgeslagen.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

Het voorbeeld toont hoe de tekstopslaginstellingen in te stellen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een instantie van indexinstellingen maken
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Instellen van een hoog compressieniveau voor de tekstopslag van de index
// Een index maken in de opgegeven map
Index index = new Index(indexFolder, settings);
// Documenten indexeren
index.add(documentsFolder);
// Zoeken
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Stelt de tekstopslaginstellingen in. De standaardwaarde is  null , wat betekent dat documentteksten niet worden opgeslagen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | De tekstopslaginstellingen. |

Het voorbeeld toont hoe de tekstopslaginstellingen in te stellen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een instantie van indexinstellingen maken
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Instellen van een hoog compressieniveau voor de tekstopslag van de index
// Een index maken in de opgegeven map
Index index = new Index(indexFolder, settings);
// Documenten indexeren
index.add(documentsFolder);
// Zoeken
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Haalt het type index op. De standaardwaarde is  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Stelt het type index in. De standaardwaarde is  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Het type index. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Haalt het aantal threads op dat voor de zoekopdracht wordt gebruikt. De standaardwaarde is  GroupDocs.Search.Options.NumberOfThreads.Default , wat betekent dat de zoekopdracht wordt uitgevoerd met een aantal threads gelijk aan het aantal processorkernen.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Stelt het aantal threads in dat voor de zoekopdracht wordt gebruikt. De standaardwaarde is  GroupDocs.Search.Options.NumberOfThreads.Default , wat betekent dat de zoekopdracht wordt uitgevoerd met een aantal threads gelijk aan het aantal processorkernen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Het aantal threads dat voor de zoekopdracht wordt gebruikt. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Haalt de collectie van aangepaste extractors op. Het volledige voorbeeld van het implementeren van een aangepaste extractor wordt gepresenteerd in de documentatie voor de  GroupDocs.Search.Common.IFieldExtractor  interface.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Haalt een logger op die wordt gebruikt voor het loggen van gebeurtenissen en fouten in de index. Merk op dat de logger niet wordt opgeslagen en elke keer dat de index wordt gemaakt of geladen, moet worden aangemaakt en toegewezen.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Stelt een logger in die wordt gebruikt voor het loggen van gebeurtenissen en fouten in de index. Merk op dat de logger niet wordt opgeslagen en elke keer dat de index wordt gemaakt of geladen moet worden aangemaakt en toegewezen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | Een logger die wordt gebruikt voor het loggen van gebeurtenissen en fouten in de index. |
|

