---
title: "SearchPhaseCompleted"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Se produit lorsque la phase de recherche est terminée."
type: docs
weight: 80
url: /fr/net/groupdocs.search.events/eventhub/searchphasecompleted/
---
## EventHub.SearchPhaseCompleted event

Se produit lorsque la phase de recherche est terminée.

```csharp
public event EventHandler<SearchPhaseEventArgs> SearchPhaseCompleted;
```

### Exemples

L'exemple montre comment utiliser l'événement.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);

// S'abonner à l'événement
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

### Voir aussi

* class [SearchPhaseEventArgs](../../searchphaseeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
