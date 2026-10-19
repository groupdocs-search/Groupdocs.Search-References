---
title: "SearchPhaseCompleted"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Si verifica quando la fase di ricerca è completata."
type: docs
weight: 80
url: /it/net/groupdocs.search.events/eventhub/searchphasecompleted/
---
## EventHub.SearchPhaseCompleted event

Si verifica quando la fase di ricerca è completata.

```csharp
public event EventHandler<SearchPhaseEventArgs> SearchPhaseCompleted;
```

### Esempi

L'esempio dimostra come utilizzare l'evento.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);

// Sottoscrizione all'evento
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

### Vedi anche

* class [SearchPhaseEventArgs](../../searchphaseeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
