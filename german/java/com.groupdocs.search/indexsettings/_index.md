---
title: "IndexSettings"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Indexeinstellungen dar, die die Anpassung der Indizierungsoperationen ermöglichen."
type: docs
weight: 19
url: /de/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Stellt die Indexeinstellungen dar, die die Anpassung der Indizierungsoperationen ermöglichen.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // Festlegen des Index-Typs
Index index = new Index(indexFolder, settings); // Erstellen eines Index
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | Initialisiert eine neue Instanz der Klasse  IndexSettings . |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | Gibt einen Wert zurück, der angibt, ob der Index im Speicher oder auf der Festplatte gespeichert ist. |
|
|  | [getUseStopWords()](#getUseStopWords--) | Gibt einen Wert zurück, der angibt, ob Stoppwörter verwendet werden sollen oder nicht. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Setzt einen Wert, der angibt, ob Stoppwörter verwendet werden sollen oder nicht. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Gibt die maximale Anzahl von Indexierungsberichten zurück. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Setzt die maximale Anzahl von Indexierungsberichten. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Gibt die maximale Anzahl von Suchberichten zurück. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Setzt die maximale Anzahl von Suchberichten. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Gibt einen Wert zurück, der angibt, ob Zeichenersetzungen verwendet werden sollen oder nicht. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Setzt einen Wert, der angibt, ob Zeichenersetzungen verwendet werden sollen oder nicht. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | Gibt einen Dokumentfilter zurück. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Setzt einen Dokumentfilter. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | Gibt die Einstellungen für die Textspeicherung zurück. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Setzt die Einstellungen für die Textspeicherung. |
|
|  | [getIndexType()](#getIndexType--) | Gibt den Index-Typ zurück. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Setzt den Index-Typ. |
|
|  | [getSearchThreads()](#getSearchThreads--) | Liefert die Anzahl der für die Suche verwendeten Threads. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Legt die Anzahl der für die Suche verwendeten Threads fest. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Liefert die benutzerdefinierte Extraktorsammlung. |
|
|  | [getLogger()](#getLogger--) | Liefert einen Logger, der zum Protokollieren von Ereignissen und Fehlern im Index verwendet wird. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Legt einen Logger fest, der zum Protokollieren von Ereignissen und Fehlern im Index verwendet wird. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Initialisiert eine neue Instanz der Klasse  IndexSettings .


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Gibt einen Wert zurück, der angibt, ob der Index im Speicher oder auf der Festplatte gespeichert ist.


**Returns:**
boolean - Ein Wert, der angibt, ob der Index im Speicher oder auf der Festplatte gespeichert wird.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Liefert einen Wert, der angibt, ob Stoppwörter verwendet werden oder nicht. Der Standardwert ist  true .


**Returns:**
boolean - Ein Wert, der angibt, ob Stoppwörter verwendet werden oder nicht.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Legt einen Wert fest, der angibt, ob Stoppwörter verwendet werden oder nicht. Der Standardwert ist  true .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob Stoppwörter verwendet werden oder nicht. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Liefert die maximale Anzahl von Indexierungsberichten. Der Standardwert ist  5 .


**Returns:**
int - Die maximale Anzahl von Indexierungsberichten.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Legt die maximale Anzahl von Indexierungsberichten fest. Der Standardwert ist  5 .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Indexierungsberichten. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Liefert die maximale Anzahl von Suchberichten. Der Standardwert ist  10 .


**Returns:**
int - Die maximale Anzahl von Suchberichten.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Legt die maximale Anzahl von Suchberichten fest. Der Standardwert ist  10 .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von Suchberichten. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Liefert einen Wert, der angibt, ob Zeichenersetzungen verwendet werden oder nicht. Der Standardwert ist  false .


**Returns:**
boolean - Ein Wert, der angibt, ob Zeichenersetzungen verwendet werden oder nicht.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Legt einen Wert fest, der angibt, ob Zeichenersetzungen verwendet werden oder nicht. Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob Zeichenersetzungen verwendet werden oder nicht. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Liefert einen Dokumentfilter. Der  DocumentFilter  arbeitet nach der Einschlusslogik. Verwenden Sie die  DocumentFilter  Klasse, um eine Dokumentfilterinstanz zu erstellen. Der Standardwert ist  null , was bedeutet, dass alle hinzugefügten Dokumente indiziert werden.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

Das Beispiel zeigt, wie man den DocumentFilter festlegt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Filters, der Dokumente mit den Erweiterungen '.doc', '.docx', '.rtf' überspringt
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Erstellen eines Dateierweiterungsfilters
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Umkehren des Dateierweiterungsfilters
settings.setDocumentFilter(invertedFilter);
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder, settings);
// Indizieren von Dokumenten
index.add(documentsFolder);
// Suchen
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Legt einen Dokumentfilter fest. Der  DocumentFilter  arbeitet nach der Einschlusslogik. Verwenden Sie die  GroupDocs.Search.Options.DocumentFilter  Klasse zur Erstellung von Dokumentfilter-Instanzen. Der Standardwert ist  null , was bedeutet, dass alle hinzugefügten Dokumente indiziert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Der Dokumentfilter. |

Das Beispiel zeigt, wie man den DocumentFilter festlegt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Filters, der Dokumente mit den Erweiterungen '.doc', '.docx', '.rtf' überspringt
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Erstellen eines Dateierweiterungsfilters
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Umkehren des Dateierweiterungsfilters
settings.setDocumentFilter(invertedFilter);
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder, settings);
// Indizieren von Dokumenten
index.add(documentsFolder);
// Suchen
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Ruft die Einstellungen für die Textspeicherung ab. Der Standardwert ist  null , was bedeutet, dass Dokumenttexte nicht gespeichert werden.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

Das Beispiel zeigt, wie die Einstellungen für die Textspeicherung festgelegt werden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen einer Indexeinstellungsinstanz
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Festlegen eines hohen Komprimierungsgrades für die Textspeicherung des Index
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder, settings);
// Indizieren von Dokumenten
index.add(documentsFolder);
// Suchen
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Legt die Einstellungen für die Textspeicherung fest. Der Standardwert ist  null , was bedeutet, dass Dokumenttexte nicht gespeichert werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | Die Einstellungen für die Textspeicherung. |

Das Beispiel zeigt, wie die Einstellungen für die Textspeicherung festgelegt werden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen einer Indexeinstellungsinstanz
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Festlegen eines hohen Komprimierungsgrades für die Textspeicherung des Index
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder, settings);
// Indizieren von Dokumenten
index.add(documentsFolder);
// Suchen
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Ruft den Indextyp ab. Der Standardwert ist  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Legt den Indextyp fest. Der Standardwert ist  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Der Indextyp. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Ruft die Anzahl der für die Suche verwendeten Threads ab. Der Standardwert ist  GroupDocs.Search.Options.NumberOfThreads.Default , was bedeutet, dass die Suche mit einer Anzahl von Threads durchgeführt wird, die der Anzahl der Prozessorkerne entspricht.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Legt die Anzahl der für die Suche verwendeten Threads fest. Der Standardwert ist  GroupDocs.Search.Options.NumberOfThreads.Default , was bedeutet, dass die Suche mit einer Anzahl von Threads durchgeführt wird, die der Anzahl der Prozessorkerne entspricht.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | Die Anzahl der für die Suche verwendeten Threads. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Ruft die Sammlung benutzerdefinierter Extraktoren ab. Das vollständige Beispiel für die Implementierung eines benutzerdefinierten Extraktors wird in der Dokumentation für die  GroupDocs.Search.Common.IFieldExtractor  Schnittstelle vorgestellt.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Ruft einen Logger ab, der zum Protokollieren von Ereignissen und Fehlern im Index verwendet wird. Beachten Sie, dass der Logger nicht gespeichert wird und jedes Mal erstellt und zugewiesen werden muss, wenn der Index erstellt oder geladen wird.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Legt einen Logger fest, der zum Protokollieren von Ereignissen und Fehlern im Index verwendet wird. Beachten Sie, dass der Logger nicht gespeichert wird und jedes Mal erstellt und zugewiesen werden muss, wenn der Index erstellt oder geladen wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | Ein Logger, der zum Protokollieren von Ereignissen und Fehlern im Index verwendet wird. |
|

