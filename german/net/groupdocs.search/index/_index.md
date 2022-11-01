---
title: Index
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Stellt die Hauptklasse dar um Dokumente zu indizieren und zu durchsuchen.
type: docs
weight: 650
url: /de/net/groupdocs.search/index/
---
## Index class

Stellt die Hauptklasse dar, um Dokumente zu indizieren und zu durchsuchen.

```csharp
public class Index : IDisposable
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [Index](index#constructor)() | Initialisiert eine neue Instanz von[`Index`](../index) Klasse im Gedächtnis. |
| [Index](index#constructor_1)(IndexSettings) | Initialisiert eine neue Instanz von[`Index`](../index) Klasse im Speicher mit bestimmten Indexeinstellungen. |
| [Index](index#constructor_2)(string) | Initialisiert eine neue Instanz von[`Index`](../index) class. Erstellt einen neuen oder öffnet einen vorhandenen Index auf der Festplatte. |
| [Index](index#constructor_3)(string, bool) | Initialisiert eine neue Instanz von[`Index`](../index) class. Lädt einen vorhandenen Index von der Festplatte, wenn*overwriteIfExists* ist`FALSCH`; erstellt andernfalls einen neuen Index auf der Festplatte. |
| [Index](index#constructor_4)(string, IndexSettings) | Initialisiert eine neue Instanz von[`Index`](../index) class. Erstellt einen neuen Index mit bestimmten Einstellungen oder öffnet einen bestehenden Index auf der Festplatte. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Initialisiert eine neue Instanz von[`Index`](../index) class. Lädt einen vorhandenen Index von der Festplatte, wenn*overwriteIfExists* ist`FALSCH` ; erstellt andernfalls einen neuen Index auf der Festplatte mit bestimmten Indexeinstellungen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Ruft das Wörterbuch-Repository ab. |
| [Events](../../groupdocs.search/index/events) { get; } | Ruft den Event Hub zum Abonnieren von Ereignissen ab. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Ruft die grundlegenden Informationen zum Index ab. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Ruft die Indexeinstellungen ab. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Ruft das Index-Repository-Objekt ab, wenn der Index darin enthalten ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Führt einen Indizierungsvorgang durch. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indiziert. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Führt einen Indizierungsvorgang durch. Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indiziert. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Führt Indizierungsoperationen durch. Fügt Dokumente aus Dateisystem, Stream oder Struktur hinzu. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Führt den Indexierungsvorgang durch. Fügt die extrahierten Daten dem Index hinzu. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Führt einen Indizierungsvorgang durch. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indiziert. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Führt einen Indizierungsvorgang durch. Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indiziert. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Wendet den angegebenen Stapel von Attributänderungen auf indizierte Dokumente an, ohne während des Aktualisierungsvorgangs neu zu indizieren. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Löscht indizierte Dateien oder Ordner aus dem Index. Aktualisiert dann den Index ohne gelöschte Pfade. Beachten Sie, dass ein einzelnes Dokument nicht aus dem Index gelöscht werden kann, wenn es dem Index als Teil eines Ordners hinzugefügt wurde. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Löscht indizierte Dokumente aus Streams oder Strukturen. Aktualisiert dann den Index ohne gelöschte Dokumente. |
| [Dispose](../../groupdocs.search/index/dispose)() | Gibt alle Ressourcen frei, die von verwendet werden[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Ruft alle Attribute ab, die dem angegebenen indizierten Dokument zugeordnet sind. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Generiert HTML-formatierten Text für das indizierte Dokument und überträgt ihn über den Ausgabeadapter. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Generiert HTML-formatierten Text für das indizierte Dokument und überträgt ihn über den Ausgabeadapter. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Ruft ein Array verschachtelter Elemente des angegebenen Dokuments ab (für Containerdokumente wie ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Ruft ein Array aller indizierten Dokumente ab. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Ruft ein Array von indizierten Pfaden ab – Dokumente oder Ordner. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Ruft die Berichte zu Indizierungsvorgängen ab. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Ruft die Berichte zu Suchvorgängen ab. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Führt den angegebenen Index mit dem aktuellen Index zusammen. Beachten Sie, dass der andere Index nicht geändert wird. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Führt Indizes aus dem angegebenen Index-Repository in den aktuellen Index zusammen. Beachten Sie, dass Indizes im Repository nicht geändert werden. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Übergibt das angegebene Benachrichtigungsobjekt an den Index, um die Benachrichtigung auszuführen. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimiert die Anzahl der Indexsegmente, indem sie miteinander verbunden werden. Dieser Vorgang verbessert die Suchleistung. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimiert die Anzahl der Indexsegmente, indem sie miteinander verbunden werden. Dieser Vorgang verbessert die Suchleistung. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Sucht im Index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Sucht im Index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Führt eine umgekehrte Bildsuche im Index durch. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Sucht im Index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Sucht im Index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Setzt die Chunk-Suche fort, die mit der Methode Search gestartet wurde. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Setzt die Chunk-Suche fort, die mit der Methode Search gestartet wurde. |
| [Update](../../groupdocs.search/index/update#update)() | Indiziert Dokumente neu, die seit der letzten Aktualisierung geändert oder gelöscht wurden. Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Indiziert Dokumente neu, die seit der letzten Aktualisierung geändert oder gelöscht wurden. Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden. |

### Bemerkungen

**Mehr erfahren**

* [Index erstellen](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indizierung](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Suchen](https://docs.groupdocs.com/display/searchnet/Searching)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

SearchResult result = index.Search(query); // Suche im Index
```

### Siehe auch

* namensraum [GroupDocs.Search](../../groupdocs.search)
* Montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
