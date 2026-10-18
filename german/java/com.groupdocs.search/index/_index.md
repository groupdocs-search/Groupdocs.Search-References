---
title: "Index"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Hauptklasse für die Indizierung von Dokumenten und die Suche darin dar."
type: docs
weight: 17
url: /de/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Stellt die Hauptklasse für die Indizierung von Dokumenten und die Suche darin dar.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchResult result = index.search(query); // Suche im Index
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Index()](#Index--) | Initialisiert eine neue Instanz der  Index  Klasse im Speicher. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Initialisiert eine neue Instanz der  Index  Klasse im Speicher mit bestimmten Indexeinstellungen. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Initialisiert eine neue Instanz der  Index  Klasse. |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Initialisiert eine neue Instanz von |
Index
Klasse.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Initialisiert eine neue Instanz von |
Index
Klasse.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Initialisiert eine neue Instanz von |
Index
Klasse.
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getEvents()](#getEvents--) | Ermittelt den Ereignis‑Hub zum Abonnieren von Ereignissen. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Ruft die grundlegenden Informationen zum Index ab. |
|
|  | [getRepository()](#getRepository--) | Ruft das Index-Repository-Objekt ab, wenn der Index darin enthalten ist. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Ruft die Indexeinstellungen ab. |
|
|  | [getDictionaries()](#getDictionaries--) | Ruft das Wörterbuch-Repository ab. |
|
|  | [close()](#close--) | Gibt alle vom System genutzten Ressourcen frei |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | Führt einen Indexierungsvorgang aus. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Führt einen Indexierungsvorgang aus. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Führt einen Indexierungsvorgang aus. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Führt einen Indexierungsvorgang aus. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Führt einen Indexierungsvorgang aus. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Führt einen Indexierungsvorgang aus. |
|
|  | [update()](#update--) | Indiziert Dokumente, die seit dem letzten Update geändert oder gelöscht wurden, neu. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Indiziert Dokumente, die seit dem letzten Update geändert oder gelöscht wurden, neu. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Ruft die Berichte zu Indexierungsvorgängen ab. |
|
|  | [getSearchReports()](#getSearchReports--) | Ruft die Berichte zu Suchvorgängen ab. |
|
|  | [search(String query)](#search-java.lang.String-) | Durchsucht den Index. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Durchsucht den Index. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Durchsucht den Index. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Durchsucht den Index. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Führt eine umgekehrte Bildsuche im Index durch. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Setzt die Chunk-Suche fort, die mit der Methode Search gestartet wurde. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Setzt die Chunk-Suche fort, die mit der Methode Search gestartet wurde. |
|
|  | [optimize()](#optimize--) | Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Führt den angegebenen Index in den aktuellen Index zusammen. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Führt Indizes aus dem angegebenen Index-Repository in den aktuellen Index zusammen. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Ruft ein Array aller indizierten Dokumente ab. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Ruft ein Array von Dokumentelementen ab. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Ruft ein indiziertes Dokument anhand des Dokumentenschlüssels ab. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Erzeugt den Text eines indizierten Dokuments und leitet ihn über einen Ausgabeadapter weiter. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Erzeugt HTML-formatierten Text für ein indiziertes Dokument und überträgt ihn über den Ausgabeadapter. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | Ruft ein Array indizierter Pfade – Dokumente oder Ordner – ab. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Löscht indizierte Dateien oder Ordner aus dem Index. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Löscht aus Streams oder Strukturen indizierte Dokumente. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Übergibt das angegebene Benachrichtigungsobjekt an den Index, um die Benachrichtigung auszuführen. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Wendet den angegebenen Batch von Attributänderungen auf indizierte Dokumente an, ohne während des Update-Vorgangs neu zu indizieren. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Ruft alle Attribute ab, die mit dem angegebenen indizierten Dokument verknüpft sind. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Lädt den gesamten Index in den Speicher. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Lädt den gesamten Index in den Speicher. |
|
### Index() {#Index--}
```
public Index()
```


Initialisiert eine neue Instanz der  Index  Klasse im Speicher.


Das Beispiel zeigt, wie man einen Index im Speicher erstellt, ohne Dateien auf die Festplatte zu speichern.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Initialisiert eine neue Instanz der  Index  Klasse im Speicher mit bestimmten Indexeinstellungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Das Indexeinstellungsobjekt. |


Das Beispiel zeigt, wie man einen Index im Speicher erstellt, ohne Dateien auf die Festplatte zu speichern, und dabei bestimmte Indexeinstellungen verwendet.

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


Initialisiert eine neue Instanz der  Index  Klasse. Erstellt ein neues oder öffnet ein vorhandenes Index auf dem Datenträger.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Der Pfad des Indexordners. |


Das Beispiel zeigt, wie man ein Index auf einem Datenträger erstellt oder ein vorhandenes Index öffnet.

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


Initialisiert eine neue Instanz von
Index
Klasse.
Erstellt ein neues Index mit bestimmten Einstellungen oder öffnet ein vorhandenes Index auf dem Datenträger.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Der Pfad des Indexordners. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Das Indexeinstellungsobjekt. |

Das Beispiel zeigt, wie man ein Index auf einem Datenträger mit bestimmten Indexeinstellungen erstellt.

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


Initialisiert eine neue Instanz von
Index
Klasse.
Lädt ein vorhandenes Index vom Datenträger, wenn
overwriteIfExists
ist
false
;
erstellt andernfalls ein neues Index auf dem Datenträger.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Der Pfad des Indexordners. |
|
|  | overwriteIfExists | boolean | Das Flag zum Überschreiben des Indexordners. |

Das Beispiel zeigt, wie man ein neues Index in einem Ordner erstellt, der bereits ein anderes Index enthält.

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


Initialisiert eine neue Instanz von
Index
Klasse.
Lädt ein vorhandenes Index vom Datenträger, wenn
overwriteIfExists
ist
false
;
erstellt andernfalls ein neues Index auf dem Datenträger mit bestimmten Indexeinstellungen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Der Pfad des Indexordners. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Das Indexeinstellungsobjekt. |
|
|  | overwriteIfExists | boolean | Das Flag zum Überschreiben des Indexordners. |

Das Beispiel zeigt, wie man ein Index auf einem Datenträger mit bestimmten Indexeinstellungen erstellt.

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


Ermittelt den Ereignis‑Hub zum Abonnieren von Ereignissen.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Ruft die grundlegenden Informationen zum Index ab.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Ruft das Index-Repository-Objekt ab, wenn der Index darin enthalten ist.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Ruft die Indexeinstellungen ab.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Ruft das Wörterbuch-Repository ab.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Gibt alle vom System genutzten Ressourcen frei
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Führt einen Indexierungsvorgang aus.
Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu.
Dokumente aus allen Unterordnern werden indiziert.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Pfad | java.lang.String | Der Pfad zu einer Datei oder einem Ordner, die indiziert werden soll. |

Das Beispiel zeigt, wie man Dokumente zu einem Index hinzufügt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(folderPath); // Indizieren von Dokumenten im angegebenen Ordner
index.add(filePath); // Indizieren des angegebenen Dokuments
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Führt einen Indexierungsvorgang aus.
Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu.
Dokumente aus allen Unterordnern werden indiziert.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Pfad | java.lang.String | Der Pfad zu einer Datei oder einem Ordner, die indiziert werden soll. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Die Indexierungsoptionen. |

Das Beispiel zeigt, wie man Dokumente zu einem Index mit bestimmten Indexierungsoptionen hinzufügt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Festlegen der Anzahl von Indexierungs-Threads
index.add(folderPath, options); // Indizieren von Dokumenten im angegebenen Ordner
index.add(filePath, options); // Indizieren des angegebenen Dokuments
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Führt einen Indexierungsvorgang aus.
Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu.
Dokumente aus allen Unterordnern werden indiziert.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | paths | java.lang.String[] | Die Pfade zu Dateien oder Ordnern, die indiziert werden sollen. |

Das Beispiel zeigt, wie man Dokumente zu einem Index hinzufügt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Indizieren von Dokumenten an den angegebenen Pfaden
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Führt einen Indexierungsvorgang aus.
Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu.
Dokumente aus allen Unterordnern werden indiziert.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | paths | java.lang.String[] | Die Pfade zu Dateien oder Ordnern, die indiziert werden sollen. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Die Indexierungsoptionen. |

Das Beispiel zeigt, wie man Dokumente zu einem Index mit bestimmten Indexierungsoptionen hinzufügt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Festlegen der Anzahl von Indexierungs-Threads
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Indizieren von Dokumenten an den angegebenen Pfaden
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Führt einen Indexierungsvorgang aus.
Fügt Dokumente aus dem Dateisystem, Stream oder einer Struktur hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Die Dokumente aus dem Dateisystem, Stream oder einer Struktur. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Die Indexierungsoptionen. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Führt einen Indexierungsvorgang aus.
Fügt die extrahierten Daten dem Index hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Die extrahierten Daten. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Die Indexierungsoptionen. |
|

### update() {#update--}
```
public final void update()
```


Indiziert Dokumente, die seit dem letzten Update geändert oder gelöscht wurden, neu.
Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden.

Das Beispiel zeigt, wie man einen Index aktualisiert.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
// Dokumente aus dem Dokumentenordner löschen oder sie ändern oder neue Dokumente zum Ordner hinzufügen
index.update(); // Aktualisieren des Index
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Indiziert Dokumente, die seit dem letzten Update geändert oder gelöscht wurden, neu.
Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Die Aktualisierungsoptionen. |

Das Beispiel zeigt, wie man einen Index mit bestimmten Aktualisierungsoptionen aktualisiert.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
// Dokumente aus dem Dokumentenordner löschen oder sie ändern oder neue Dokumente zum Ordner hinzufügen
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Festlegen der Anzahl von Indexierungs-Threads
index.update(options); // Aktualisieren des Index
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Ruft die Berichte zu Indexierungsvorgängen ab.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - Die Indexierungsberichte.

Das Beispiel zeigt, wie man Indexierungsberichte abruft.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
IndexingReport[] reports = index.getIndexingReports(); // Abrufen von Indexierungsberichten
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Ruft die Berichte zu Suchvorgängen ab.


**Returns:**
com.groupdocs.search.common.SearchReport[] - Die Suchberichte.

Das Beispiel zeigt, wie man Suchberichte erhält.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchResult result1 = index.search(query1); // Suchen
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // Abrufen von Suchberichten
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Durchsucht den Index.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | java.lang.String | Die Suchanfrage. |

Das folgende Beispiel zeigt, wie man eine einfache Suche durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchResult result = index.search(query); // Suchen
 
```
 
````

Das folgende Beispiel zeigt, wie man eine Regex-Suche durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
String query = "^[0-9]{3,}"; // Das Zirkumflex‑Symbol am Anfang der Suchanfrage teilt dem Index mit, dass es sich um eine Regex‑Abfrage handelt
SearchResult result = index.search(query); // Suchen
 
```
 
````

Das folgende Beispiel zeigt, wie man eine facettierte Suche durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
String query = "content:Newton"; // Das Wort vor dem Doppelpunkt in der Abfrage bedeutet den Namen des zu durchsuchenden Dokumentfeldes
SearchResult result = index.search(query); // Suchen
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Durchsucht den Index.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | java.lang.String | Die Suchanfrage. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Die Suchoptionen. |

Das folgende Beispiel zeigt, wie man eine unscharfe Suche durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Aktivieren der unscharfen Suche
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Festlegen der maximalen Anzahl möglicher Unterschiede pro Wort
// Anführungszeichen am Anfang und Ende teilen dem Index mit, dass es sich um eine Phrasensuchanfrage handelt
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // Suche
 
```
 
````

Das folgende Beispiel zeigt, wie man eine Synonymsuche durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Aktivieren der Synonymsuche
String query = "cry";
SearchResult result = index.search(query, options); // Suche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Durchsucht den Index.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Die Suchanfrage. |

Das folgende Beispiel zeigt, wie man eine Suche mit einer Abfrage in Objektform durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
// Erstellen von Unterabfrage 1
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // Festlegen der Suchoptionen nur für Unterabfrage 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Aktivieren der unscharfen Suche
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Festlegen der maximalen Anzahl von Unterschieden
// Erstellen von Unterabfrage 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Erstellen von Unterabfrage 3
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// Kombinieren von Unterabfragen zu einer Abfrage
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Suchen
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Durchsucht den Index.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Die Suchanfrage. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Die Suchoptionen. |

Das folgende Beispiel zeigt, wie man eine Suche mit einer Abfrage in Objektform durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
// Erstellen einer Unterabfrage für die Datumsspanne-Suche
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// Erstellen einer Unterabfrage für Wildcard mit einer Anzahl fehlender Wörter von 0 bis 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// Erstellen einer Unterabfrage für ein einfaches Wort
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Festlegen der Suchoptionen nur für Unterabfrage 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// Kombinieren von Unterabfragen zu einer Abfrage
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// Erstellen eines Suchoptionen-Objekts mit erhöhter Kapazität gefundener Vorkommen
SearchOptions options = new SearchOptions(); // Gesamte Suchoptionen
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // Suche
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Führt eine umgekehrte Bildsuche im Index durch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Das Bild zum Durchsuchen. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Die Bildsuchoptionen. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Setzt die Chunk-Suche fort, die mit der Methode Search gestartet wurde.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Das Chunk-Such-Token. |

Das Beispiel zeigt, wie man eine Chunk‑Suche durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Aktivieren der Chunk‑Suche
SearchResult result = index.search(query, options); // Starten der Chunk‑Suche
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Fortsetzen der Chunk‑Suche
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


Setzt die Chunk-Suche fort, die mit der Methode Search gestartet wurde.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Das Chunk-Such-Token. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | Das Abbruchobjekt. |

Das Beispiel zeigt, wie man die Suche mit einer Abfrage in Objektform durchführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
Cancellation cancellation = new Cancellation(); // Dieses Abbruchobjekt bricht alle Suchfortsetzungen ab, wenn es abgebrochen wird
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Aktivieren der Chunk‑Suche
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Starten der Chunk‑Suche
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Fortsetzen der Chunk‑Suche
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


Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden.
Dieser Vorgang verbessert die Suchleistung.

Das Beispiel zeigt, wie man Segmente eines Index zusammenführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder1); // Indizierung von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder2); // Jeder Aufruf von AddToIndex erstellt mindestens ein neues Segment im Index
index.add(documentsFolder3);
// Zusammenführen von Segmenten des Index
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden.
Dieser Vorgang verbessert die Suchleistung.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Die Merge-Optionen. |

Das Beispiel zeigt, wie man Segmente eines Index mit bestimmten Merge-Optionen zusammenführt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Erstellen des Index im angegebenen Ordner
index.add(documentsFolder1); // Indizierung von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder2); // Jeder Aufruf von AddToIndex erstellt mindestens ein neues Segment im Index
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // Asynchroner Vorgang
options.setCancellation(new Cancellation()); // Erstellen eines Abbruchobjekts
// Zusammenführen von Segmenten des Index
index.optimize(options); // Diese Methode kehrt zurück, bevor der Vorgang abgeschlossen ist
options.getCancellation().cancelAfter(10000); // Festlegen der maximalen Dauer des Vorgangs auf 10 Sekunden
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Führt den angegebenen Index in den aktuellen Index zusammen.
Beachten Sie, dass der andere Index nicht geändert wird.


Wenn der andere Index eine vorherige Version hat, muss er vor dem Zusammenführen aktualisiert werden
IndexUpdater
.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Der Index, in den zusammengeführt werden soll. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Die Merge-Optionen. |

Das Beispiel zeigt, wie man einen Index in den aktuellen Index zusammenführt.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // Erstellen von index1
index1.add(documentsFolder1); // Indizieren von Dokumenten
Index index2 = new Index(indexFolder2); // Erstellen von index2
index2.add(documentsFolder2); // Indizieren von Dokumenten
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Erstellen eines Abbruchobjekts
// Zusammenführen von index2 in index1. Beachten Sie, dass index2-Dateien nicht geändert werden.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Führt Indizes aus dem angegebenen Index-Repository in den aktuellen Index zusammen.
Beachten Sie, dass Indizes im Repository nicht geändert werden.


Wenn andere Indizes eine vorherige Version haben, müssen sie vor dem Zusammenführen mit
IndexUpdater
.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | Das Index-Repository, in das zusammengeführt werden soll. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Die Merge-Optionen. |

Das Beispiel zeigt, wie ein Index-Repository in den aktuellen Index zusammengeführt wird.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // Erstellen von index1
index1.add(documentsFolder1); // Indizieren von Dokumenten
IndexRepository repository = new IndexRepository(); // Erstellen des Index-Repositorys
Index index2 = repository.create(indexFolder2); // Erstellen von index2
index2.add(documentsFolder2); // Indizieren von Dokumenten
Index index3 = repository.create(indexFolder3); // Erstellen von index3
index3.add(documentsFolder3); // Indizieren von Dokumenten
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Erstellen eines Abbruchobjekts
// Zusammenführen aller Indizes im Index-Repository in index1. Beachten Sie, dass index2 und index3 nicht geändert werden.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Das gefundene Dokument. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Der Hervorheber für Suchergebnisse. |

Das Beispiel zeigt, wie Vorkommen in HTML-formatiertem Text hervorgehoben werden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentFolder);
// Suchen nach dem Wort 'eternity'
SearchResult result = index.search("eternity");
// Hervorheben von Vorkommen im Text
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Abrufen des ersten gefundenen Dokuments
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Erstellen eines Output-Adapters für die Datei
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Erstellen des Highlighter-Objekts
index.highlight(document, highlighter); // Generieren von HTML-formatiertem Text mit hervorgehobenen Vorkommen
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Das gefundene Dokument. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Der Hervorheber für Suchergebnisse. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Die Hervorhebungsoptionen. |

Das Beispiel zeigt, wie Vorkommen in HTML-formatiertem Text hervorgehoben werden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentFolder);
// Suchen nach dem Wort 'eternity'
SearchResult result = index.search("eternity");
// Hervorheben von Vorkommen im Text
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Abrufen des ersten gefundenen Dokuments
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Erstellen eines Output-Adapters für die Datei
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Erstellen des Highlighter-Objekts
HighlightOptions options = new HighlightOptions(); // Erstellen des Hervorhebungsoptionen-Objekts
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // Generieren von HTML-formatiertem Text mit hervorgehobenen Vorkommen
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Ruft ein Array aller indizierten Dokumente ab.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Ein Array aller indizierten Dokumente.

Das Beispiel zeigt, wie man eine Liste indizierter Dokumente aus einem Index erhält.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
// Abrufen der Liste indizierter Dokumente
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Ruft ein Array von Dokumentelementen ab.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Eine Dokumentinformation. |

Das Beispiel zeigt, wie man eine Liste von Elementen eines indizierten Dokuments aus einem Index erhält.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
// Abrufen der Liste indizierter Dokumente
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Abrufen der Liste von Dokumentelementen
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Ein Array von Dokumentelementen.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Ruft ein indiziertes Dokument anhand des Dokumentenschlüssels ab.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentKey | java.lang.String | Der Dokumentenschlüssel. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Erzeugt den Text eines indizierten Dokuments und leitet ihn über einen Ausgabeadapter weiter.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Die indizierte Dokumentinformation. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Der Ausgabeadapter. |

Das Beispiel zeigt, wie man den Text eines indizierten Dokuments aus einem Index erhält.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
// Abrufen der Liste indizierter Dokumente
DocumentInfo[] documents = index.getIndexedDocuments();
// Abrufen eines Dokumenttexts
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


Erzeugt HTML-formatierten Text für ein indiziertes Dokument und überträgt ihn über den Ausgabeadapter.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Die indizierte Dokumentinformation. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Der Ausgabeadapter. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | Die Optionen zum Abrufen von Text. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Ruft ein Array indizierter Pfade – Dokumente oder Ordner – ab.


**Returns:**
java.lang.String[] - Ein Array von indizierten Pfaden.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Löscht indizierte Dateien oder Ordner aus dem Index. Aktualisiert anschließend den Index ohne die gelöschten Pfade.
Beachten Sie, dass ein einzelnes Dokument nicht aus dem Index gelöscht werden kann, wenn es als Teil eines Ordners zum Index hinzugefügt wurde.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | paths | java.lang.String[] | Die Pfade zu Dateien oder Ordnern, die gelöscht werden sollen. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Die Aktualisierungsoptionen. |

Das Beispiel zeigt, wie indizierte Pfade aus einem Index gelöscht werden können.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus den angegebenen Ordnern
index.add(documentsFolder1);
index.add(documentsFolder2);
// Abrufen indizierter Pfade aus dem Index
String[] indexedPaths1 = index.getIndexedPaths();
// Schreiben indizierter Pfade in die Konsole
System.out.println("Indizierte Pfade:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// Löschen eines Indexpfads aus dem Index
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Abrufen indizierter Pfade nach dem Löschen
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nGelöschte Pfade: " + deleteResult.getSuccessCount());
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


Löscht Dokumente, die aus Streams oder Strukturen indiziert wurden. Aktualisiert dann den Index ohne gelöschte Dokumente.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Die Aktualisierungsoptionen. |
|
|  | documentKeys | java.lang.String[] | Die Schlüssel der aus Streams oder Strukturen hinzugefügten Dokumente. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Übergibt das angegebene Benachrichtigungsobjekt an den Index, um die Benachrichtigung auszuführen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | Das Benachrichtigungsobjekt. |
|

**Returns:**
boolean - Gibt  true  zurück, wenn die Benachrichtigung erfolgreich durchgeführt wurde; andernfalls  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Wendet den angegebenen Batch von Attributänderungen auf indizierte Dokumente an, ohne während des Update-Vorgangs neu zu indizieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Das Batch für Attributänderungen. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Ruft alle Attribute ab, die mit dem angegebenen indizierten Dokument verknüpft sind.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Pfad | java.lang.String | Der Dokumentpfad. |
|

**Returns:**
java.lang.String[] - Mit dem Dokument verbundene Attribute.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Lädt den gesamten Index in den Speicher.
Alle Änderungen am Index werden nicht automatisch im ursprünglichen Ordner gespeichert.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Der Pfad des Indexordners. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Lädt den gesamten Index in den Speicher.
Alle Änderungen am Index werden nicht automatisch im ursprünglichen Ordner gespeichert.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Der Pfad des Indexordners. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Das Indexeinstellungsobjekt. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

