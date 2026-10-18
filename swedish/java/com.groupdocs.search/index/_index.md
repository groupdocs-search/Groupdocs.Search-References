---
title: "Index"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar huvudklassen för indexering av dokument och sökning genom dem."
type: docs
weight: 17
url: /sv/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Representerar huvudklassen för indexering av dokument och sökning genom dem.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchResult result = index.search(query); // Söker i index
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Index()](#Index--) | Initierar en ny instans av  Index  klassen i minnet. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Initierar en ny instans av  Index  klassen i minnet med särskilda indexinställningar. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Initierar en ny instans av  Index  klassen. |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Initierar en ny instans av |
Index
klassen.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Initierar en ny instans av |
Index
klassen.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Initierar en ny instans av |
Index
klassen.
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getEvents()](#getEvents--) | Hämtar händelsehubben för att prenumerera på händelser. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Hämtar grundläggande information om indexet. |
|
|  | [getRepository()](#getRepository--) | Hämtar indexförrådsobjektet om indexet finns i det. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Hämtar indexinställningarna. |
|
|  | [getDictionaries()](#getDictionaries--) | Hämtar ordförrådet. |
|
|  | [close()](#close--) | Frigör alla resurser som används av |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | Utför indexeringsoperation. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Utför indexeringsoperation. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Utför indexeringsoperation. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Utför indexeringsoperation. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Utför indexeringsoperation. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Utför indexeringsoperation. |
|
|  | [update()](#update--) | Indexerar om dokument som har ändrats eller raderats sedan senaste uppdateringen. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Indexerar om dokument som har ändrats eller raderats sedan senaste uppdateringen. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Hämtar rapporterna om indexeringsoperationer. |
|
|  | [getSearchReports()](#getSearchReports--) | Hämtar rapporterna om sökoperationer. |
|
|  | [search(String query)](#search-java.lang.String-) | Söker i index. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Söker i index. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Söker i index. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Söker i index. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Utför en omvänd bildsökning i index. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Fortsätter chunk-sökningen som startades med metoden Search. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Fortsätter chunk-sökningen som startades med metoden Search. |
|
|  | [optimize()](#optimize--) | Minimerar antalet indexsegment genom att slå samman dem ett med ett. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Minimerar antalet indexsegment genom att slå samman dem ett med ett. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Slår samman det angivna indexet med det aktuella indexet. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Slår samman index från det angivna indexförrådet med det aktuella indexet. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Genererar HTML-formaterad text med markerade hittade termer. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Genererar HTML-formaterad text med markerade hittade termer. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Hämtar en array med alla indexerade dokument. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Hämtar en array med dokumentobjekt. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Hämtar ett indexerat dokument med dokumentnyckel. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Genererar texten för ett indexerat dokument och skickar den genom en utdataadapter. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Genererar HTML-formaterad text för ett indexerat dokument och överför den genom utdataadaptern. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | Hämtar en array med indexerade sökvägar – dokument eller mappar. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Tar bort indexerade filer eller mappar från index. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Tar bort dokument som indexerats från strömmar eller strukturer. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Skickar det angivna notifikationsobjektet till indexet för att utföra notifikationen. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Tillämpar den angivna batchen av attributändringar på indexerade dokument utan omindexering under uppdateringsoperationen. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Hämtar alla attribut som är associerade med det angivna indexerade dokumentet. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Laddar hela indexet i minnet. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Laddar hela indexet i minnet. |
|
### Index() {#Index--}
```
public Index()
```


Initierar en ny instans av  Index  klassen i minnet.


Exemplet visar hur man skapar ett index i minnet utan att spara filer på disk.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Initierar en ny instans av  Index  klassen i minnet med särskilda indexinställningar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Indexinställningsobjektet. |


Exemplet visar hur man skapar ett index i minnet utan att spara filer på disk med särskilda indexinställningar.

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


Initierar en ny instans av Index-klassen. Skapar ett nytt eller öppnar ett befintligt index på disk.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Sökvägen till indexmappen. |


Exemplet visar hur man skapar ett index på en disk eller öppnar ett befintligt index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


Initierar en ny instans av
Index
klassen.
Skapar ett nytt index med specifika inställningar eller öppnar ett befintligt index på disk.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Sökvägen till indexmappen. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Indexinställningsobjektet. |

Exemplet visar hur man skapar ett index på en disk med specifika indexinställningar.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


Initierar en ny instans av
Index
klassen.
Laddar ett befintligt index från disk om
overwriteIfExists
är
false
;
skapar ett nytt index på disk annars.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Sökvägen till indexmappen. |
|
|  | overwriteIfExists | boolean | Flaggan för att skriva över indexmappen. |

Exemplet visar hur man skapar ett nytt index i en mapp som redan innehåller ett annat index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


Initierar en ny instans av
Index
klassen.
Laddar ett befintligt index från disk om
overwriteIfExists
är
false
;
skapar ett nytt index på disk med specifika indexinställningar annars.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Sökvägen till indexmappen. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Indexinställningsobjektet. |
|
|  | overwriteIfExists | boolean | Flaggan för att skriva över indexmappen. |

Exemplet visar hur man skapar ett index på en disk med specifika indexinställningar.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Hämtar händelsehubben för att prenumerera på händelser.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Hämtar grundläggande information om indexet.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Hämtar indexförrådsobjektet om indexet finns i det.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Hämtar indexinställningarna.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Hämtar ordförrådet.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Frigör alla resurser som används av
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Utför indexeringsoperation.
Lägger till en fil eller mapp med en absolut eller relativ sökväg.
Dokument från alla undermappar kommer att indexeras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökväg | java.lang.String | Sökvägen till en fil eller mapp som ska indexeras. |

Exemplet visar hur man lägger till dokument i ett index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(folderPath); // Indexerar dokument i den angivna mappen
index.add(filePath); // Indexerar det angivna dokumentet
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Utför indexeringsoperation.
Lägger till en fil eller mapp med en absolut eller relativ sökväg.
Dokument från alla undermappar kommer att indexeras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökväg | java.lang.String | Sökvägen till en fil eller mapp som ska indexeras. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Indexeringsalternativen. |

Exemplet visar hur man lägger till dokument i ett index med särskilda indexeringsalternativ.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Ställer in antalet indexeringstrådar
index.add(folderPath, options); // Indexerar dokument i den angivna mappen
index.add(filePath, options); // Indexerar det angivna dokumentet
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Utför indexeringsoperation.
Lägger till filer eller mappar med en absolut eller relativ sökväg.
Dokument från alla undermappar kommer att indexeras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökvägar | java.lang.String[] | Sökvägarna till filer eller mappar som ska indexeras. |

Exemplet visar hur man lägger till dokument i ett index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Indexerar dokument på de angivna sökvägarna
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Utför indexeringsoperation.
Lägger till filer eller mappar med en absolut eller relativ sökväg.
Dokument från alla undermappar kommer att indexeras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökvägar | java.lang.String[] | Sökvägarna till filer eller mappar som ska indexeras. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Indexeringsalternativen. |

Exemplet visar hur man lägger till dokument i ett index med särskilda indexeringsalternativ.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Ställer in antalet indexeringstrådar
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Indexerar dokument på de angivna sökvägarna
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Utför indexeringsoperation.
Lägger till dokument från filsystem, ström eller struktur.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Dokumenten från filsystem, ström eller struktur. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Indexeringsalternativen. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Utför indexeringsoperation.
Lägger till den extraherade datan i indexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Den extraherade datan. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Indexeringsalternativen. |
|

### update() {#update--}
```
public final void update()
```


Indexerar om dokument som har ändrats eller raderats sedan senaste uppdateringen.
Lägger till nya filer som har lagts till i de indexerade mapparna.

Exemplet visar hur man uppdaterar ett index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
// Radera dokument från dokumentmappen eller ändra dem eller lägg till nya dokument i mappen
index.update(); // Uppdaterar indexet
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Indexerar om dokument som har ändrats eller raderats sedan senaste uppdateringen.
Lägger till nya filer som har lagts till i de indexerade mapparna.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Uppdateringsalternativen. |

Exemplet visar hur man uppdaterar ett index med särskilda uppdateringsalternativ.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
// Radera dokument från dokumentmappen eller ändra dem eller lägg till nya dokument i mappen
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Ställer in antalet indexeringstrådar
index.update(options); // Uppdaterar indexet
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Hämtar rapporterna om indexeringsoperationer.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - Indexeringsrapporterna.

Exemplet visar hur man hämtar indexeringsrapporter.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
IndexingReport[] reports = index.getIndexingReports(); // Hämtar indexeringsrapporter
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Hämtar rapporterna om sökoperationer.


**Returns:**
com.groupdocs.search.common.SearchReport[] - Sökrapporterna.

Exemplet visar hur man hämtar sökrapporter.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchResult result1 = index.search(query1); // Söker
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // Hämtar sökrapporter
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Söker i index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | java.lang.String | Sökfrågan. |

Följande exempel visar hur man utför en enkel sökning.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchResult result = index.search(query); // Söker
 
```
 
````

Följande exempel visar hur man utför en Regex-sökning.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
String query = "^[0-9]{3,}"; // Caret-symbolen i början av sökfrågan talar om för indexet att det är en Regex-fråga
SearchResult result = index.search(query); // Söker
 
```
 
````

Följande exempel visar hur man utför en fasetterad sökning.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
String query = "content:Newton"; // Ordet före kolon i frågan betyder dokumentfältets namn att söka i
SearchResult result = index.search(query); // Söker
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Söker i index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | java.lang.String | Sökfrågan. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Sökalternativen. |

Följande exempel visar hur man utför en fuzzy-sökning.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Aktiverar fuzzy-sökning
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Ställer in antalet möjliga skillnader för varje ord
// Dubbelcitat i början och slutet talar om för indexet att det är en fras-sökfråga
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // Söker
 
```
 
````

Följande exempel visar hur man utför en synonym-sökning.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Aktiverar synonym-sökning
String query = "cry";
SearchResult result = index.search(query, options); // Söker
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Söker i index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Sökfrågan. |

Följande exempel visar hur man utför en sökning med fråga i objektform.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
// Skapar delfråga 1
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // Ställer in sökalternativ endast för delfråga 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Aktiverar fuzzy-sökning
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Ställer in maximalt antal skillnader
// Skapar delfråga 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Skapar delfråga 3
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// Kombinerar delfrågor till en fråga
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Söker
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Söker i index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Sökfrågan. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Sökalternativen. |

Följande exempel visar hur man utför en sökning med fråga i objektform.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
// Skapar delfråga för datumintervallssökning
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// Skapar delfråga för jokertecken med antal missade ord från 0 till 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// Skapar delfråga för enkelt ord
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Ställer in sökalternativ endast för delfråga 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// Kombinerar delfrågor till en fråga
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// Skapar sökalternativobjekt med ökad kapacitet för funna förekomster
SearchOptions options = new SearchOptions(); // Övergripande sökalternativ
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // Söker
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Utför en omvänd bildsökning i index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Bilden att söka. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Sökalternativen för bilden. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Fortsätter chunk-sökningen som startades med metoden Search.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Chunk-sökningstoken. |

Exemplet visar hur man utför chunk-sökning.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Aktiverar chunk-sökning
SearchResult result = index.search(query, options); // Startar chunk-sökning
System.out.println("Antal dokument: " + result.getDocumentCount());
System.out.println("Antal förekomster: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Fortsätter chunk-sökning
System.out.println("Antal dokument: " + result.getDocumentCount());
System.out.println("Antal förekomster: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


Fortsätter chunk-sökningen som startades med metoden Search.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Chunk-sökningstoken. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | Avbrytningsobjektet. |

Exemplet visar hur man utför sökning med query i objektform.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
Cancellation cancellation = new Cancellation(); // Detta avbrytningsobjekt avbryter alla sökfortsättningar om det avbryts
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Aktiverar chunk-sökning
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Startar chunk-sökning
System.out.println("Antal dokument: " + result.getDocumentCount());
System.out.println("Antal förekomster: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Fortsätter chunk-sökning
System.out.println("Antal dokument: " + result.getDocumentCount());
System.out.println("Antal förekomster: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


Minimerar antalet indexsegment genom att slå samman dem ett med ett.
Denna operation förbättrar sökprestanda.

Exemplet visar hur man slår ihop segment av ett index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder1); // Indexerar dokument från den angivna mappen
index.add(documentsFolder2); // Varje anrop till AddToIndex skapar minst ett nytt segment i indexet
index.add(documentsFolder3);
// Sammanfogar segment i indexet
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Minimerar antalet indexsegment genom att slå samman dem ett med ett.
Denna operation förbättrar sökprestanda.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Sammanfogningsalternativen. |

Exemplet visar hur man sammanfogar segment i ett index med särskilda sammanfogningsalternativ.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.add(documentsFolder1); // Indexerar dokument från den angivna mappen
index.add(documentsFolder2); // Varje anrop till AddToIndex skapar minst ett nytt segment i indexet
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // Asynkron operation
options.setCancellation(new Cancellation()); // Skapar avbokningsobjekt
// Sammanfogar segment i indexet
index.optimize(options); // Denna metod returnerar innan operationen är slutförd
options.getCancellation().cancelAfter(10000); // Ställer in maximal varaktighet för operationen till 10 sekunder
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Slår samman det angivna indexet med det aktuella indexet.
Observera att det andra indexet inte kommer att ändras.


Om det andra indexet har en tidigare version måste det uppdateras innan sammanslagning med
IndexUpdater
.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Indexet att slå samman med. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Sammanfogningsalternativen. |

Exemplet visar hur man slår samman ett index med det aktuella indexet.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // Skapar index1
index1.add(documentsFolder1); // Indexerar dokument
Index index2 = new Index(indexFolder2); // Skapar index2
index2.add(documentsFolder2); // Indexerar dokument
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Skapar avbokningsobjekt
// Sammanfogar index2 i index1. Observera att index2-filerna inte kommer att ändras.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Slår samman index från det angivna indexförrådet med det aktuella indexet.
Observera att index i lagret inte kommer att ändras.


Om andra index har en tidigare version måste de uppdateras innan sammanslagning med
IndexUpdater
.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | Indexlagret att slå samman med. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Sammanfogningsalternativen. |

Exemplet visar hur man slår samman ett indexlager med det aktuella indexet.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // Skapar index1
index1.add(documentsFolder1); // Indexerar dokument
IndexRepository repository = new IndexRepository(); // Skapar indexlager
Index index2 = repository.create(indexFolder2); // Skapar index2
index2.add(documentsFolder2); // Indexerar dokument
Index index3 = repository.create(indexFolder3); // Skapar index3
index3.add(documentsFolder3); // Indexerar dokument
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Skapar avbokningsobjekt
// Slår samman alla index i indexlagret med index1. Observera att index2 och index3 inte kommer att ändras.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Genererar HTML-formaterad text med markerade hittade termer.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Det hittade dokumentet. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Sökresultatets markerare. |

Exemplet visar hur man markerar förekomster i HTML-formaterad text.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentFolder);
// Sök efter ordet 'eternity'
SearchResult result = index.search("eternity");
// Markerar förekomster i text
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Hämtar det första hittade dokumentet
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Skapar en utdataadapter till filen
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Skapar markeringsobjektet
index.highlight(document, highlighter); // Genererar HTML-formaterad text med markerade förekomster
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Genererar HTML-formaterad text med markerade hittade termer.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Det hittade dokumentet. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Sökresultatets markerare. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Markeringsalternativen. |

Exemplet visar hur man markerar förekomster i HTML-formaterad text.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentFolder);
// Sök efter ordet 'eternity'
SearchResult result = index.search("eternity");
// Markerar förekomster i text
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Hämtar det första hittade dokumentet
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Skapar en utdataadapter till filen
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Skapar markeringsobjektet
HighlightOptions options = new HighlightOptions(); // Skapar markeringsalternativobjektet
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // Genererar HTML-formaterad text med markerade förekomster
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Hämtar en array med alla indexerade dokument.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - En array av alla indexerade dokument.

Exemplet visar hur man får en lista över indexerade dokument från ett index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
// Hämtar lista över indexerade dokument
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Hämtar en array med dokumentobjekt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | En dokumentinformation. |

Exemplet visar hur man får en lista över objekt i ett indexerat dokument från ett index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
// Hämtar lista över indexerade dokument
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Hämtar lista över dokumentobjekt
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - En array av dokumentobjekt.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Hämtar ett indexerat dokument med dokumentnyckel.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentKey | java.lang.String | Dokumentnyckeln. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Genererar texten för ett indexerat dokument och skickar den genom en utdataadapter.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Den indexerade dokumentinformationen. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Utdataadaptern. |

Exemplet visar hur man får texten från ett indexerat dokument från ett index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
// Hämtar lista över indexerade dokument
DocumentInfo[] documents = index.getIndexedDocuments();
// Hämtar en dokumenttext
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


Genererar HTML-formaterad text för ett indexerat dokument och överför den genom utdataadaptern.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Den indexerade dokumentinformationen. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Utdataadaptern. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | Alternativen för att hämta text. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Hämtar en array med indexerade sökvägar – dokument eller mappar.


**Returns:**
java.lang.String[] - En array av indexerade sökvägar.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Tar bort indexerade filer eller mappar från indexet. Uppdaterar sedan indexet utan de borttagna sökvägarna.
Observera att ett enskilt dokument inte kan tas bort från indexet om det lades till i indexet som en del av en mapp.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökvägar | java.lang.String[] | Sökvägarna till filer eller mappar som ska tas bort. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Uppdateringsalternativen. |

Exemplet visar hur man tar bort indexerade sökvägar från ett index.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
// Indexerar dokument från de angivna mapparna
index.add(documentsFolder1);
index.add(documentsFolder2);
// Hämtar indexerade sökvägar från indexet
String[] indexedPaths1 = index.getIndexedPaths();
// Skriver indexerade sökvägar till konsolen
System.out.println("Indexerade sökvägar:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// Tar bort indexväg från indexet
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Hämtar indexerade sökvägar efter borttagning
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nBorttagna sökvägar: " + deleteResult.getSuccessCount());
System.out.println("\nIndexed paths:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


Tar bort dokument som indexerats från strömmar eller strukturer. Uppdaterar sedan indexet utan de borttagna dokumenten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Uppdateringsalternativen. |
|
|  | documentKeys | java.lang.String[] | Nycklarna för dokument som lagts till från strömmar eller strukturer. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Skickar det angivna notifikationsobjektet till indexet för att utföra notifikationen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | Meddelandesobjektet. |
|

**Returns:**
boolean - Returnerar  true  om meddelandet lyckades; annars  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Tillämpar den angivna batchen av attributändringar på indexerade dokument utan omindexering under uppdateringsoperationen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Batchen för attributändringar. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Hämtar alla attribut som är associerade med det angivna indexerade dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökväg | java.lang.String | Dokumentets sökväg. |
|

**Returns:**
java.lang.String[] - Attribut som är associerade med dokumentet.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Laddar hela indexet i minnet.
Eventuella ändringar i indexet sparas inte automatiskt till den ursprungliga mappen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Sökvägen till indexmappen. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Laddar hela indexet i minnet.
Eventuella ändringar i indexet sparas inte automatiskt till den ursprungliga mappen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Sökvägen till indexmappen. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Indexinställningsobjektet. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

