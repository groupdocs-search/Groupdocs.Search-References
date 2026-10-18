---
title: "SearchPhaseCompleted"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Tritt auf, wenn die Suchphase abgeschlossen ist."
type: docs
weight: 80
url: /de/net/groupdocs.search.events/eventhub/searchphasecompleted/
---
## EventHub.SearchPhaseCompleted event

Tritt auf, wenn die Suchphase abgeschlossen ist.

```csharp
public event EventHandler<SearchPhaseEventArgs> SearchPhaseCompleted;
```

### Beispiele

Das Beispiel zeigt, wie das Ereignis verwendet wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);

// Abonnieren des Ereignisses
index.Events.SearchPhaseCompleted += (sender, args) =>
{
    Console.WriteLine("Search phase: " + args.SearchPhase);
    Console.WriteLine("Words: " + args.Words.Length);
};

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true;
options.UseWordFormsSearch = true;
options.FuzzySearch.Enabled = true;
options.UseHomophoneSearch = true;
SearchResult result = index.Search("Einstein", options);
```

### Siehe auch

* class [SearchPhaseEventArgs](../../searchphaseeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
