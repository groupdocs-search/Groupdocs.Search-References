---
title: "IndexSettings"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar indexinställningarna som möjliggör anpassning av indexeringsoperationer."
type: docs
weight: 19
url: /sv/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Representerar indexinställningarna som möjliggör anpassning av indexeringsoperationer.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Ställer in indextypen
Index index = new Index(indexFolder, settings); // Skapar ett index
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | Initierar en ny instans av klassen IndexSettings. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Hämtar ett värde som indikerar om indexet lagras i minnet eller på disk. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Hämtar ett värde som indikerar om stoppord ska användas eller inte. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Ställer in ett värde som indikerar om stoppord ska användas eller inte. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Hämtar det maximala antalet indexeringsrapporter. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Ställer in det maximala antalet indexeringsrapporter. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Hämtar det maximala antalet sökrapporter. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Ställer in det maximala antalet sökrapporter. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Hämtar ett värde som indikerar om teckenersättningar ska användas eller inte. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Ställer in ett värde som indikerar om teckenersättningar ska användas eller inte. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Hämtar ett dokumentfilter. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Ställer in ett dokumentfilter. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Hämtar textlagringsinställningarna. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Ställer in textlagringsinställningarna. |
|
|  | [getIndexType()](#getIndexType--) | Hämtar indextypen. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Ställer in indextypen. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Hämtar antalet trådar som används för sökningen. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Ställer in antalet trådar som används för sökningen. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Hämtar den anpassade extrahörssamlingen. |
|
|  | [getLogger()](#getLogger--) | Hämtar en logger som används för att logga händelser och fel i indexet. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Ställer in en logger som används för att logga händelser och fel i indexet. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Initierar en ny instans av klassen IndexSettings.


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Hämtar ett värde som indikerar om indexet lagras i minnet eller på disk.


**Returns:**
boolean - Ett värde som indikerar om indexet lagras i minnet eller på disk.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Hämtar ett värde som indikerar om stoppord ska användas eller inte. Standardvärdet är  true .


**Returns:**
boolean - Ett värde som indikerar om stoppord ska användas eller inte.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Ställer in ett värde som indikerar om stoppord ska användas eller inte. Standardvärdet är  true .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om stoppord ska användas eller inte. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Hämtar det maximala antalet indexeringsrapporter. Standardvärdet är  5 .


**Returns:**
int - Det maximala antalet indexeringsrapporter.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Ställer in det maximala antalet indexeringsrapporter. Standardvärdet är  5 .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet indexeringsrapporter. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Hämtar det maximala antalet sökrapporter. Standardvärdet är  10 .


**Returns:**
int - Det maximala antalet sökrapporter.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Ställer in det maximala antalet sökrapporter. Standardvärdet är  10 .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet sökrapporter. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Hämtar ett värde som indikerar om teckenersättningar ska användas eller inte. Standardvärdet är  false .


**Returns:**
boolean - Ett värde som indikerar om teckenersättningar ska användas eller inte.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Ställer in ett värde som indikerar om teckenersättningar ska användas eller inte. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om teckenersättningar ska användas eller inte. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Hämtar ett dokumentfilter.  DocumentFilter  fungerar enligt inklusionslogiken. Använd  DocumentFilter  -klassen för att skapa en instans av ett dokumentfilter. Standardvärdet är  null , vilket betyder att alla tillagda dokument indexeras.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

Exemplet visar hur man ställer in dokumentfiltret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett filter som hoppar över dokument med filändelserna '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Skapar filter för filändelser
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Inverterar filter för filändelser
settings.setDocumentFilter(invertedFilter);
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder, settings);
// Indexerar dokument
index.add(documentsFolder);
// Söker
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Ställer in ett dokumentfilter. DocumentFilter fungerar med inklusionslogik. Använd klassen GroupDocs.Search.Options.DocumentFilter för att skapa instanser av ett dokumentfilter. Standardvärdet är null, vilket betyder att alla tillagda dokument indexeras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Dokumentfiltret. |

Exemplet visar hur man ställer in dokumentfiltret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett filter som hoppar över dokument med filändelserna '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Skapar filter för filändelser
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Inverterar filter för filändelser
settings.setDocumentFilter(invertedFilter);
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder, settings);
// Indexerar dokument
index.add(documentsFolder);
// Söker
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Hämtar inställningarna för textlagring. Standardvärdet är null, vilket betyder att dokumenttexter inte lagras.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

Exemplet visar hur man ställer in inställningarna för textlagring.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar instans av indexinställningar
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Ställer in hög komprimeringsnivå för indexets textlagring
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder, settings);
// Indexerar dokument
index.add(documentsFolder);
// Söker
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Ställer in inställningarna för textlagring. Standardvärdet är null, vilket betyder att dokumenttexter inte lagras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | Inställningarna för textlagring. |

Exemplet visar hur man ställer in inställningarna för textlagring.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar instans av indexinställningar
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Ställer in hög komprimeringsnivå för indexets textlagring
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder, settings);
// Indexerar dokument
index.add(documentsFolder);
// Söker
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Hämtar indextypen. Standardvärdet är GroupDocs.Search.Options.IndexType.NormalIndex.


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Ställer in indextypen. Standardvärdet är GroupDocs.Search.Options.IndexType.NormalIndex.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Indextypen. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Hämtar antalet trådar som används för sökningen. Standardvärdet är GroupDocs.Search.Options.NumberOfThreads.Default, vilket betyder att sökningen utförs med ett antal trådar lika med antalet processorkärnor.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Ställer in antalet trådar som används för sökningen. Standardvärdet är GroupDocs.Search.Options.NumberOfThreads.Default, vilket betyder att sökningen utförs med ett antal trådar lika med antalet processorkärnor.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Antalet trådar som används för sökningen. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Hämtar samlingen av anpassade extrahörer. Det fullständiga exemplet på implementering av en anpassad extrahör presenteras i dokumentationen för gränssnittet GroupDocs.Search.Common.IFieldExtractor.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Hämtar en logger som används för att logga händelser och fel i indexet. Observera att loggern inte sparas och måste skapas och tilldelas varje gång indexet skapas eller laddas.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Ställer in en logger som används för att logga händelser och fel i indexet. Observera att loggern inte sparas och måste skapas och tilldelas varje gång indexet skapas eller laddas.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | En logger som används för att logga händelser och fel i indexet. |
|

