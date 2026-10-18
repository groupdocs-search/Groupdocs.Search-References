---
title: "Index"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt die Hauptklasse zum Indexieren von Dokumenten und Durchsuchen dieser dar."
type: docs
weight: 700
url: /de/net/groupdocs.search/index/
---
## Index class

Stellt die Hauptklasse zum Indexieren von Dokumenten und Durchsuchen dieser dar.

```csharp
public class Index : IDisposable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Index](index#constructor)() | Initialisiert eine neue Instanz der [`Index`](../index)-Klasse im Speicher. |
| [Index](index#constructor_1)(IndexSettings) | Initialisiert eine neue Instanz der [`Index`](../index)-Klasse im Speicher mit bestimmten Indexeinstellungen. |
| [Index](index#constructor_2)(string) | Initialisiert eine neue Instanz der [`Index`](../index)-Klasse. Erstellt einen neuen Index oder öffnet einen vorhandenen Index auf der Festplatte. |
| [Index](index#constructor_3)(string, bool) | Initialisiert eine neue Instanz der [`Index`](../index)-Klasse. Lädt einen vorhandenen Index von der Festplatte, wenn *overwriteIfExists* `false` ist; erstellt andernfalls einen neuen Index auf der Festplatte. |
| [Index](index#constructor_4)(string, IndexSettings) | Initialisiert eine neue Instanz der [`Index`](../index)-Klasse. Erstellt einen neuen Index mit bestimmten Einstellungen oder öffnet einen vorhandenen Index auf der Festplatte. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Initialisiert eine neue Instanz der [`Index`](../index)-Klasse. Lädt einen vorhandenen Index von der Festplatte, wenn *overwriteIfExists* `false` ist; erstellt andernfalls einen neuen Index auf der Festplatte mit bestimmten Indexeinstellungen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Ruft das Wörterbuch-Repository ab. |
| [Events](../../groupdocs.search/index/events) { get; } | Liefert den Ereignis-Hub zum Abonnieren von Ereignissen. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Ruft die grundlegenden Informationen zum Index ab. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Ruft die Indexeinstellungen ab. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Ruft das Index-Repository-Objekt ab, falls der Index darin enthalten ist. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Lädt den gesamten Index in den Speicher. Änderungen am Index werden nicht automatisch im ursprünglichen Ordner gespeichert. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Lädt den gesamten Index in den Speicher. Änderungen am Index werden nicht automatisch im ursprünglichen Ordner gespeichert. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Führt einen Indexierungsvorgang aus. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indexiert. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Führt einen Indexierungsvorgang aus. Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indexiert. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Führt einen Indexierungsvorgang aus. Fügt Dokumente aus dem Dateisystem, Stream oder einer Struktur hinzu. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Führt einen Indexierungsvorgang aus. Fügt die extrahierten Daten dem Index hinzu. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Führt einen Indexierungsvorgang aus. Fügt eine Datei oder einen Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indexiert. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Führt einen Indexierungsvorgang aus. Fügt Dateien oder Ordner über einen absoluten oder relativen Pfad hinzu. Dokumente aus allen Unterordnern werden indexiert. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Wendet das angegebene Batch von Attributänderungen auf indexierte Dokumente an, ohne während des Update-Vorgangs neu zu indexieren. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Überprüft den Index auf beschädigte Segmentdateien auf der Festplatte. Die Methode repariert die Indexfunktionalität bei beschädigten Segmenten, wenn *fixIndexFunctionality* wahr ist; andernfalls wird nicht repariert. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Löscht indexierte Dateien oder Ordner aus dem Index. Aktualisiert anschließend den Index ohne die gelöschten Pfade. Hinweis: Ein einzelnes Dokument kann nicht aus dem Index gelöscht werden, wenn es als Teil eines Ordners zum Index hinzugefügt wurde. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Löscht aus Streams oder Strukturen indexierte Dokumente. Aktualisiert anschließend den Index ohne die gelöschten Dokumente. |
| [Dispose](../../groupdocs.search/index/dispose)() | Gibt alle von der [`Index`](../index) genutzten Ressourcen frei. |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Ruft alle Attribute ab, die dem angegebenen indexierten Dokument zugeordnet sind. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Erzeugt den Text eines indexierten Dokuments und leitet ihn über einen Ausgabeadapter weiter. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Erzeugt HTML-formatierten Text für ein indexiertes Dokument und überträgt ihn über den Ausgabeadapter. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Ruft ein indexiertes Dokument anhand des Dokumentenschlüssels ab. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Gibt ein Array verschachtelter Elemente des angegebenen Dokuments zurück (für Container-Dokumente wie ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Gibt ein Array aller indizierten Dokumente zurück. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Gibt ein Array indizierter Pfade zurück – Dokumente oder Ordner. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Gibt die Berichte zu Indexierungsvorgängen zurück. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Gibt die Berichte zu Suchvorgängen zurück. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Führt den angegebenen Index in den aktuellen Index zusammen. Hinweis: Der andere Index wird nicht geändert. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Führt Indizes aus dem angegebenen Index-Repository in den aktuellen Index zusammen. Hinweis: Die Indizes im Repository werden nicht geändert. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Übergibt das angegebene Benachrichtigungsobjekt an den Index, um die Benachrichtigung auszuführen. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. Dieser Vorgang verbessert die Suchleistung. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. Dieser Vorgang verbessert die Suchleistung. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Speichert den In‑Memory‑Index auf die Festplatte. Speichert außerdem den regulären Index in einen anderen Ordner. Ändert die Einstellungen dieses Index nicht. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Durchsucht den Index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Durchsucht den Index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Führt eine umgekehrte Bildsuche im Index durch. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Durchsucht den Index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Durchsucht den Index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Setzt die Chunk‑Suche fort, die mit der Methode Search gestartet wurde. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Setzt die Chunk‑Suche fort, die mit der Methode Search gestartet wurde. |
| [Update](../../groupdocs.search/index/update#update)() | Indiziert Dokumente, die seit dem letzten Update geändert oder gelöscht wurden, neu. Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Indiziert Dokumente, die seit dem letzten Update geändert oder gelöscht wurden, neu. Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden. |

### Hinweise

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### Siehe auch

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
