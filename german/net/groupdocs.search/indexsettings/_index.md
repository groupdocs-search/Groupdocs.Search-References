---
title: "IndexSettings"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt die Indexeinstellungen dar, die die Anpassung der Indexierungsvorgänge ermöglichen."
type: docs
weight: 720
url: /de/net/groupdocs.search/indexsettings/
---
## IndexSettings class

Stellt die Indexeinstellungen dar, die die Anpassung der Indexierungsvorgänge ermöglichen.

```csharp
public class IndexSettings
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [IndexSettings](indexsettings)() | Initialisiert eine neue Instanz der [`IndexSettings`](../indexsettings)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CustomExtractors](../../groupdocs.search/indexsettings/customextractors) { get; } | Ruft die benutzerdefinierte Extraktor‑Sammlung ab. |
| [DocumentFilter](../../groupdocs.search/indexsettings/documentfilter) { get; set; } | Ruft einen Dokumentfilter ab oder legt ihn fest. Der [`DocumentFilter`](./documentfilter) arbeitet nach der Einschlusslogik. Verwenden Sie die [`DocumentFilter`](../../groupdocs.search.options/documentfilter)-Klasse zur Erstellung von Dokumentfilter‑Instanzen. Der Standardwert ist `null`, was bedeutet, dass alle hinzugefügten Dokumente indiziert werden. |
| [IndexType](../../groupdocs.search/indexsettings/indextype) { get; set; } | Ruft den Indextyp ab oder legt ihn fest. Der Standardwert ist NormalIndex. |
| [InMemoryIndex](../../groupdocs.search/indexsettings/inmemoryindex) { get; } | Ruft einen Wert ab, der angibt, ob der Index im Speicher oder auf der Festplatte gespeichert ist. |
| [Logger](../../groupdocs.search/indexsettings/logger) { get; set; } | Ruft einen Logger ab oder legt ihn fest, der zum Protokollieren von Ereignissen und Fehlern im Index verwendet wird. Hinweis: Der Logger wird nicht gespeichert und muss jedes Mal erstellt und zugewiesen werden, wenn der Index erstellt oder geladen wird. |
| [MaxIndexingReportCount](../../groupdocs.search/indexsettings/maxindexingreportcount) { get; set; } | Ruft die maximale Anzahl von Indexierungsberichten ab oder legt sie fest. Der Standardwert ist `5`. |
| [MaxSearchReportCount](../../groupdocs.search/indexsettings/maxsearchreportcount) { get; set; } | Ruft die maximale Anzahl von Suchberichten ab oder legt sie fest. Der Standardwert ist `10`. |
| [SearchThreads](../../groupdocs.search/indexsettings/searchthreads) { get; set; } | Ruft die Anzahl der für die Suche verwendeten Threads ab oder legt sie fest. Der Standardwert ist Default, was bedeutet, dass die Suche mit einer Thread‑Anzahl durchgeführt wird, die der Anzahl der Prozessorkerne entspricht. |
| [TextStorageSettings](../../groupdocs.search/indexsettings/textstoragesettings) { get; set; } | Ruft die Einstellungen für die Textspeicherung ab oder legt sie fest. Der Standardwert ist `null`, was bedeutet, dass Dokumenttexte nicht gespeichert werden. |
| [UseCharacterReplacements](../../groupdocs.search/indexsettings/usecharacterreplacements) { get; set; } | Ruft einen Wert ab oder legt ihn fest, der angibt, ob Zeichenersetzungen verwendet werden sollen oder nicht. Der Standardwert ist `false`. |
| [UseStopWords](../../groupdocs.search/indexsettings/usestopwords) { get; set; } | Ruft einen Wert ab oder legt ihn fest, der angibt, ob Stoppwörter verwendet werden sollen oder nicht. Der Standardwert ist `true`. |

### Hinweise

**Learn more**

* [Search index settings](https://docs.groupdocs.com/display/searchnet/Search+index+settings)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex; // Setting the index type

Index index = new Index(indexFolder, settings); // Creating an index
```

### Siehe auch

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
