---
title: "Index"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de hoofdklasse voor het indexeren van documenten en zoeken daarin voor."
type: docs
weight: 17
url: /nl/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Stelt de hoofdklasse voor het indexeren van documenten en zoeken daarin voor.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchResult result = index.search(query); // Zoeken in index
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Index()](#Index--) | Initialiseert een nieuw exemplaar van de  Index  klasse in het geheugen. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Initialiseert een nieuw exemplaar van de  Index  klasse in het geheugen met specifieke indexinstellingen. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Initialiseert een nieuw exemplaar van de  Index  klasse. |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Initialiseert een nieuw exemplaar van de |
Index
klasse.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Initialiseert een nieuw exemplaar van de |
Index
klasse.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Initialiseert een nieuw exemplaar van de |
Index
klasse.
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getEvents()](#getEvents--) | Haalt de event-hub op voor het abonneren op gebeurtenissen. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Haalt de basisinformatie op over de index. |
|
|  | [getRepository()](#getRepository--) | Haalt het indexopslagobject op als de index erin is opgenomen. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Haalt de indexinstellingen op. |
|
|  | [getDictionaries()](#getDictionaries--) | Haalt de woordenboekopslag op. |
|
|  | [close()](#close--) | Geeft alle bronnen vrij die door de |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | Voert een indexeerbewerking uit. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Voert een indexeerbewerking uit. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Voert een indexeerbewerking uit. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Voert een indexeerbewerking uit. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Voert een indexeerbewerking uit. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Voert een indexeerbewerking uit. |
|
|  | [update()](#update--) | Indexeert documenten opnieuw die sinds de laatste update zijn gewijzigd of verwijderd. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Indexeert documenten opnieuw die sinds de laatste update zijn gewijzigd of verwijderd. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Haalt de rapporten over indexeerbewerkingen op. |
|
|  | [getSearchReports()](#getSearchReports--) | Haalt de rapporten over zoekbewerkingen op. |
|
|  | [search(String query)](#search-java.lang.String-) | Zoekt in de index. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Zoekt in de index. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Zoekt in de index. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Zoekt in de index. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Voert een omgekeerde afbeeldingzoekopdracht uit in de index. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Vervolg de blokzoekopdracht die gestart is met de methode Search. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Vervolg de blokzoekopdracht die gestart is met de methode Search. |
|
|  | [optimize()](#optimize--) | Minimaliseert het aantal indexsegmenten door ze één voor één samen te voegen. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Minimaliseert het aantal indexsegmenten door ze één voor één samen te voegen. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Voegt de opgegeven index samen met de huidige index. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Voegt indexen uit de opgegeven indexrepository samen met de huidige index. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Haalt een array op van alle geïndexeerde documenten. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Haalt een array op van documentitems. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Haalt een geïndexeerd document op op basis van de documentsleutel. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Genereert de tekst van een geïndexeerd document en geeft deze door aan een outputadapter. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Genereert HTML-geformatteerde tekst voor een geïndexeerd document en stuurt deze door via de outputadapter. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | Haalt een array op van geïndexeerde paden - documenten of mappen. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Verwijdert geïndexeerde bestanden of mappen uit de index. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Verwijdert documenten die geïndexeerd zijn vanuit streams of structuren. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Geeft het opgegeven notificatieobject door aan de index om de notificatie uit te voeren. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Past de opgegeven batch van attribuutwijzigingen toe op geïndexeerde documenten zonder opnieuw te indexeren tijdens de updatebewerking. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Haalt alle attributen op die geassocieerd zijn met het opgegeven geïndexeerde document. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Laadt de volledige index in het geheugen. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Laadt de volledige index in het geheugen. |
|
### Index() {#Index--}
```
public Index()
```


Initialiseert een nieuw exemplaar van de  Index  klasse in het geheugen.


Het voorbeeld toont hoe een index in het geheugen te maken zonder bestanden op schijf op te slaan.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Initialiseert een nieuw exemplaar van de  Index  klasse in het geheugen met specifieke indexinstellingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Het indexinstellingenobject. |


Het voorbeeld toont hoe een index in het geheugen te maken zonder bestanden op schijf op te slaan met specifieke indexinstellingen.

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


Initialiseert een nieuw exemplaar van de  Index  klasse. Maakt een nieuwe of opent een bestaande index op schijf.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Het pad van de indexmap. |


Het voorbeeld toont hoe een index op een schijf te maken of een bestaande index te openen.

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


Initialiseert een nieuw exemplaar van de
Index
klasse.
Maakt een nieuwe index met specifieke instellingen of opent een bestaande index op schijf.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Het pad van de indexmap. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Het indexinstellingenobject. |

Het voorbeeld toont hoe een index op een schijf te maken met specifieke indexinstellingen.

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


Initialiseert een nieuw exemplaar van de
Index
klasse.
Laadt een bestaande index van schijf als
overwriteIfExists
is
false
;
maakt een nieuwe index op schijf anders.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Het pad van de indexmap. |
|
|  | overwriteIfExists | boolean | De vlag voor het overschrijven van de indexmap. |

Het voorbeeld toont hoe een nieuwe index te maken in een map die al een andere index bevat.

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


Initialiseert een nieuw exemplaar van de
Index
klasse.
Laadt een bestaande index van schijf als
overwriteIfExists
is
false
;
maakt een nieuwe index op schijf met specifieke indexinstellingen anders.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Het pad van de indexmap. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Het indexinstellingenobject. |
|
|  | overwriteIfExists | boolean | De vlag voor het overschrijven van de indexmap. |

Het voorbeeld toont hoe een index op een schijf te maken met specifieke indexinstellingen.

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


Haalt de event-hub op voor het abonneren op gebeurtenissen.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Haalt de basisinformatie op over de index.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Haalt het indexopslagobject op als de index erin is opgenomen.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Haalt de indexinstellingen op.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Haalt de woordenboekopslag op.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Geeft alle bronnen vrij die door de
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Voert een indexeerbewerking uit.
Voegt een bestand of map toe via een absoluut of relatief pad.
Documenten uit alle submappen worden geïndexeerd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pad | java.lang.String | Het pad naar een bestand of map die geïndexeerd moet worden. |

Het voorbeeld toont hoe documenten aan een index toe te voegen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(folderPath); // Documenten indexeren in de opgegeven map
index.add(filePath); // Het opgegeven document indexeren
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Voert een indexeerbewerking uit.
Voegt een bestand of map toe via een absoluut of relatief pad.
Documenten uit alle submappen worden geïndexeerd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pad | java.lang.String | Het pad naar een bestand of map die geïndexeerd moet worden. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | De indexeeropties. |

Het voorbeeld toont hoe documenten aan een index kunnen worden toegevoegd met specifieke indexeeropties.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Instellen van het aantal indexeer‑threads
index.add(folderPath, options); // Documenten indexeren in de opgegeven map
index.add(filePath, options); // Het opgegeven document indexeren
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Voert een indexeerbewerking uit.
Voegt bestanden of mappen toe via een absoluut of relatief pad.
Documenten uit alle submappen worden geïndexeerd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | paths | java.lang.String[] | De paden naar bestanden of mappen die geïndexeerd moeten worden. |

Het voorbeeld toont hoe documenten aan een index toe te voegen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Documenten indexeren op de opgegeven paden
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Voert een indexeerbewerking uit.
Voegt bestanden of mappen toe via een absoluut of relatief pad.
Documenten uit alle submappen worden geïndexeerd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | paths | java.lang.String[] | De paden naar bestanden of mappen die geïndexeerd moeten worden. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | De indexeeropties. |

Het voorbeeld toont hoe documenten aan een index kunnen worden toegevoegd met specifieke indexeeropties.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Instellen van het aantal indexeer‑threads
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Documenten indexeren op de opgegeven paden
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Voert een indexeerbewerking uit.
Voegt documenten toe vanuit het bestandssysteem, een stream of een structuur.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | De documenten uit het bestandssysteem, een stream of een structuur. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | De indexeeropties. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Voert een indexeerbewerking uit.
Voegt de geëxtraheerde gegevens toe aan de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | De geëxtraheerde gegevens. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | De indexeeropties. |
|

### update() {#update--}
```
public final void update()
```


Indexeert documenten opnieuw die sinds de laatste update zijn gewijzigd of verwijderd.
Voegt nieuwe bestanden toe die aan de geïndexeerde mappen zijn toegevoegd.

Het voorbeeld toont hoe een index kan worden bijgewerkt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
// Verwijder documenten uit de documentmap of wijzig ze of voeg nieuwe documenten toe aan de map
index.update(); // De index bijwerken
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Indexeert documenten opnieuw die sinds de laatste update zijn gewijzigd of verwijderd.
Voegt nieuwe bestanden toe die aan de geïndexeerde mappen zijn toegevoegd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | De update‑opties. |

Het voorbeeld toont hoe een index kan worden bijgewerkt met specifieke update-opties.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
// Verwijder documenten uit de documentmap of wijzig ze of voeg nieuwe documenten toe aan de map
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Instellen van het aantal indexeer‑threads
index.update(options); // De index bijwerken
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Haalt de rapporten over indexeerbewerkingen op.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - De indexeer-rapporten.

Het voorbeeld toont hoe indexeer-rapporten kunnen worden opgehaald.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
IndexingReport[] reports = index.getIndexingReports(); // Indexeer-rapporten ophalen
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Haalt de rapporten over zoekbewerkingen op.


**Returns:**
com.groupdocs.search.common.SearchReport[] - De zoekrapporten.

Het voorbeeld laat zien hoe u zoekrapporten kunt ophalen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchResult result1 = index.search(query1); // Zoeken
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // Ophalen van zoekrapporten
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Zoekt in de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | java.lang.String | De zoekopdracht. |

Het volgende voorbeeld laat zien hoe u eenvoudige zoekopdrachten uitvoert.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchResult result = index.search(query); // Zoeken
 
```
 
````

Het volgende voorbeeld laat zien hoe u een Regex-zoekopdracht uitvoert.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
String query = "^[0-9]{3,}"; // Het caret-symbool aan het begin van de zoekopdracht vertelt de index dat het een Regex-query is
SearchResult result = index.search(query); // Zoeken
 
```
 
````

Het volgende voorbeeld laat zien hoe u gefacetteerd zoeken uitvoert.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
String query = "content:Newton"; // Het woord vóór de dubbele punt in de query betekent de documentveldnaam om te doorzoeken
SearchResult result = index.search(query); // Zoeken
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Zoekt in de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | java.lang.String | De zoekopdracht. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | De zoekopties. |

Het volgende voorbeeld laat zien hoe u fuzzy-zoekopdracht uitvoert.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Fuzzy-zoekopdracht inschakelen
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Instellen van het aantal mogelijke verschillen per woord
// Dubbele aanhalingstekens aan het begin en einde vertellen de index dat het een phrase search query is
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // Zoeken
 
```
 
````

Het volgende voorbeeld laat zien hoe u synoniem zoeken uitvoert.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Synoniem zoeken inschakelen
String query = "cry";
SearchResult result = index.search(query, options); // Zoeken
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Zoekt in de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | De zoekopdracht. |

Het volgende voorbeeld laat zien hoe u zoeken uitvoert met een query in objectvorm.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
// Subquery 1 aanmaken
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // Zoekopties instellen alleen voor subquery 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Fuzzy-zoekopdracht inschakelen
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Maximum aantal verschillen instellen
// Subquery 2 maken
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Subquery 3 maken
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// Subqueries combineren tot één query
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Zoeken
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Zoekt in de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | De zoekopdracht. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | De zoekopties. |

Het volgende voorbeeld laat zien hoe u zoeken uitvoert met een query in objectvorm.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
// Subquery maken voor datumreeks zoekopdracht
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// Subquery maken voor wildcard met aantal gemiste woorden van 0 tot 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// Subquery maken voor eenvoudig woord
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Zoekopties instellen alleen voor subquery 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// Subqueries combineren tot één query
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// Zoekopties-object maken met verhoogde capaciteit voor gevonden voorkomens
SearchOptions options = new SearchOptions(); // Algemene zoekopties
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // Zoeken
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Voert een omgekeerde afbeeldingzoekopdracht uit in de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | De afbeelding om te zoeken. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | De zoekopties voor de afbeelding. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Vervolg de blokzoekopdracht die gestart is met de methode Search.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Het chunk-zoektoken. |

Het voorbeeld toont hoe een chunk-zoekopdracht uit te voeren.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Chunk-zoekopdracht inschakelen
SearchResult result = index.search(query, options); // Chunk-zoekopdracht starten
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Chunk-zoekopdracht voortzetten
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
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


Vervolg de blokzoekopdracht die gestart is met de methode Search.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Het chunk-zoektoken. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | Het annuleringsobject. |

Het voorbeeld toont hoe een zoekopdracht uit te voeren met een query in objectvorm.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
Cancellation cancellation = new Cancellation(); // Dit annuleringsobject stopt alle zoekvoortzettingen als het wordt geannuleerd
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Chunk-zoekopdracht inschakelen
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Chunk-zoekopdracht starten
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Chunk-zoekopdracht voortzetten
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
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


Minimaliseert het aantal indexsegmenten door ze één voor één samen te voegen.
Deze bewerking verbetert de zoekprestaties.

Het voorbeeld toont hoe segmenten van een index te combineren.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder1); // Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder2); // Elke aanroep van AddToIndex maakt ten minste één nieuw segment in de index aan
index.add(documentsFolder3);
// Segmenten van de index samenvoegen
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Minimaliseert het aantal indexsegmenten door ze één voor één samen te voegen.
Deze bewerking verbetert de zoekprestaties.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | De samenvoegopties. |

Het voorbeeld toont hoe segmenten van een index te samenvoegen met specifieke samenvoegopties.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Index aanmaken in de opgegeven map
index.add(documentsFolder1); // Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder2); // Elke aanroep van AddToIndex maakt ten minste één nieuw segment in de index aan
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // Asynchrone bewerking
options.setCancellation(new Cancellation()); // Annuleringsobject maken
// Segmenten van de index samenvoegen
index.optimize(options); // Deze methode keert terug voordat de bewerking is voltooid
options.getCancellation().cancelAfter(10000); // Maximale duur van de bewerking instellen op 10 seconden
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Voegt de opgegeven index samen met de huidige index.
Let op: de andere index zal niet worden gewijzigd.


Als de andere index een vorige versie heeft, moet deze worden bijgewerkt voordat er wordt samengevoegd met
IndexUpdater
.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | De index waarin wordt samengevoegd. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | De samenvoegopties. |

Het voorbeeld toont hoe een index te samenvoegen met de huidige index.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // Index1 maken
index1.add(documentsFolder1); // Documenten indexeren
Index index2 = new Index(indexFolder2); // Index2 maken
index2.add(documentsFolder2); // Documenten indexeren
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Annuleringsobject maken
// index2 samenvoegen met index1. Let op: index2-bestanden zullen niet worden gewijzigd.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Voegt indexen uit de opgegeven indexrepository samen met de huidige index.
Merk op dat indexen in de repository niet worden gewijzigd.


Als andere indexen een vorige versie hebben, moeten ze worden bijgewerkt voordat ze worden samengevoegd met
IndexUpdater
.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | De indexrepository om in te voegen. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | De samenvoegopties. |

Het voorbeeld laat zien hoe een indexrepository te combineren met de huidige index.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // Index1 maken
index1.add(documentsFolder1); // Documenten indexeren
IndexRepository repository = new IndexRepository(); // Een indexrepository maken
Index index2 = repository.create(indexFolder2); // index2 maken
index2.add(documentsFolder2); // Documenten indexeren
Index index3 = repository.create(indexFolder3); // index3 maken
index3.add(documentsFolder3); // Documenten indexeren
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Annuleringsobject maken
// Alle indexen in de indexrepository samenvoegen in index1. Merk op dat index2 en index3 niet worden gewijzigd.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Het gevonden document. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | De markeerder voor zoekresultaten. |

Het voorbeeld laat zien hoe voorkomens te markeren in HTML-geformatteerde tekst.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentFolder);
// Zoeken naar het woord 'eternity'
SearchResult result = index.search("eternity");
// Voorkomens markeren in tekst
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Het eerste gevonden document ophalen
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Een outputadapter naar het bestand maken
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Een highlighter-object maken
index.highlight(document, highlighter); // HTML-tekst genereren met gemarkeerde vermeldingen
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Het gevonden document. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | De markeerder voor zoekresultaten. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | De highlight-opties. |

Het voorbeeld laat zien hoe voorkomens te markeren in HTML-geformatteerde tekst.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentFolder);
// Zoeken naar het woord 'eternity'
SearchResult result = index.search("eternity");
// Voorkomens markeren in tekst
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Het eerste gevonden document ophalen
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Een outputadapter naar het bestand maken
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Een highlighter-object maken
HighlightOptions options = new HighlightOptions(); // Een highlight-opties-object maken
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // HTML-tekst genereren met gemarkeerde vermeldingen
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Haalt een array op van alle geïndexeerde documenten.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Een array van alle geïndexeerde documenten.

Het voorbeeld laat zien hoe je een lijst met geïndexeerde documenten uit een index haalt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken in de opgegeven map
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
// Lijst met geïndexeerde documenten ophalen
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Haalt een array op van documentitems.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Een documentinfo. |

Het voorbeeld laat zien hoe je een lijst met items van een geïndexeerd document uit een index haalt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken in de opgegeven map
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
// Lijst met geïndexeerde documenten ophalen
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Lijst met documentitems ophalen
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Een array van documentitems.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Haalt een geïndexeerd document op op basis van de documentsleutel.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentKey | java.lang.String | De documentsleutel. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Genereert de tekst van een geïndexeerd document en geeft deze door aan een outputadapter.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | De geïndexeerde documentinfo. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | De output-adapter. |

Het voorbeeld laat zien hoe je de tekst van een geïndexeerd document uit een index haalt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken in de opgegeven map
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
// Lijst met geïndexeerde documenten ophalen
DocumentInfo[] documents = index.getIndexedDocuments();
// Een documenttekst ophalen
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


Genereert HTML-geformatteerde tekst voor een geïndexeerd document en stuurt deze door via de outputadapter.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | De geïndexeerde documentinfo. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | De output-adapter. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | De opties voor het ophalen van tekst. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Haalt een array op van geïndexeerde paden - documenten of mappen.


**Returns:**
java.lang.String[] - Een array van geïndexeerde paden.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Verwijdert geïndexeerde bestanden of mappen uit de index. Werkt vervolgens de index bij zonder de verwijderde paden.
Merk op dat een individueel document niet uit de index kan worden verwijderd als het als onderdeel van een map aan de index is toegevoegd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | paths | java.lang.String[] | De paden naar bestanden of mappen die moeten worden verwijderd. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | De update‑opties. |

Het voorbeeld toont hoe geïndexeerde paden uit een index kunnen worden verwijderd.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Een index maken in de opgegeven map
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven mappen
index.add(documentsFolder1);
index.add(documentsFolder2);
// Ophalen van geïndexeerde paden uit de index
String[] indexedPaths1 = index.getIndexedPaths();
// Geïndexeerde paden naar de console schrijven
System.out.println("Geïndexeerde paden:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// Indexpad verwijderen uit de index
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Ophalen van geïndexeerde paden na verwijdering
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nVerwijderde paden: " + deleteResult.getSuccessCount());
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


Verwijdert documenten die zijn geïndexeerd vanuit streams of structuren. Werk vervolgens de index bij zonder verwijderde documenten.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | De update‑opties. |
|
|  | documentKeys | java.lang.String[] | De sleutels van documenten die zijn toegevoegd vanuit streams of structuren. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Geeft het opgegeven notificatieobject door aan de index om de notificatie uit te voeren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | Het notificatieobject. |
|

**Returns:**
boolean - Retourneert  true  als de notificatie succesvol is uitgevoerd; anders  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Past de opgegeven batch van attribuutwijzigingen toe op geïndexeerde documenten zonder opnieuw te indexeren tijdens de updatebewerking.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | De batch voor attribuutwijzigingen. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Haalt alle attributen op die geassocieerd zijn met het opgegeven geïndexeerde document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pad | java.lang.String | Het documentpad. |
|

**Returns:**
java.lang.String[] - Attributen die aan het document zijn gekoppeld.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Laadt de volledige index in het geheugen.
Alle wijzigingen in de index worden niet automatisch opgeslagen in de oorspronkelijke map.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Het pad van de indexmap. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Laadt de volledige index in het geheugen.
Alle wijzigingen in de index worden niet automatisch opgeslagen in de oorspronkelijke map.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Het pad van de indexmap. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Het indexinstellingenobject. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

