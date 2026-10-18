---
title: "IndexRepository"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Container zum Kombinieren mehrerer Indizes und zum Ausführen gemeinsamer Operationen auf ihnen dar."
type: docs
weight: 710
url: /de/net/groupdocs.search/indexrepository/
---
## IndexRepository class

Stellt einen Container zum Kombinieren mehrerer Indizes und zum Ausführen gemeinsamer Operationen auf ihnen dar.

```csharp
public class IndexRepository : IDisposable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [IndexRepository](indexrepository)() | Initialisiert eine neue Instanz der [`IndexRepository`](../indexrepository)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Events](../../groupdocs.search/indexrepository/events) { get; } | Liefert den Ereignis-Hub zum Abonnieren von Ereignissen. |
| [Indexes](../../groupdocs.search/indexrepository/indexes) { get; } | Liefert die in diesem [`IndexRepository`](../indexrepository) enthaltenen Indizes. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository)(Index) | Fügt dem Index-Repository einen Index hinzu. |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository_1)(string) | Öffnet und fügt dem Index-Repository einen Index hinzu. |
| [Create](../../groupdocs.search/indexrepository/create#create)() | Erstellt einen neuen Index im Speicher. |
| [Create](../../groupdocs.search/indexrepository/create#create_1)(IndexSettings) | Erstellt einen neuen Index im Speicher. |
| [Create](../../groupdocs.search/indexrepository/create#create_2)(string) | Erstellt einen neuen Index auf der Festplatte. Der Indexordner wird vor der Erstellung des Index bereinigt. |
| [Create](../../groupdocs.search/indexrepository/create#create_3)(string, IndexSettings) | Erstellt einen neuen Index auf der Festplatte. Der Indexordner wird vor der Erstellung des Index bereinigt. |
| [Dispose](../../groupdocs.search/indexrepository/dispose)() | Gibt alle von dem [`IndexRepository`](../indexrepository) genutzten Ressourcen frei. |
| [Search](../../groupdocs.search/indexrepository/search#search)(SearchQuery) | Durchsucht alle Indizes des Repositories. |
| [Search](../../groupdocs.search/indexrepository/search#search_2)(string) | Durchsucht alle Indizes des Repositories. |
| [Search](../../groupdocs.search/indexrepository/search#search_1)(SearchQuery, SearchOptions) | Durchsucht alle Indizes des Repositories. |
| [Search](../../groupdocs.search/indexrepository/search#search_3)(string, SearchOptions) | Durchsucht alle Indizes des Repositories. |
| [Update](../../groupdocs.search/indexrepository/update#update)() | Aktualisiert alle Indizes im Repository. |
| [Update](../../groupdocs.search/indexrepository/update#update_1)(UpdateOptions) | Aktualisiert alle Indizes im Repository. |

### Hinweise

**Learn more**

* [Search index repository](https://docs.groupdocs.com/display/searchnet/Search+index+repository)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder1 = @"c:\MyIndex\";
string indexFolder2 = @"c:\MyIndex\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
repository.AddToRepository(indexFolder1); // Loading an existing index
repository.AddToRepository(indexFolder2); // Loading another existing index

SearchResult result = repository.Search(query); // Searching in indexes of the repository
```

### Siehe auch

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
