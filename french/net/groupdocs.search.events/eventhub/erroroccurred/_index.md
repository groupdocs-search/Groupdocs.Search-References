---
title: "ErrorOccurred"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Se produit lorsqu'une erreur survient lors d'une opération d'index."
type: docs
weight: 10
url: /fr/net/groupdocs.search.events/eventhub/erroroccurred/
---
## EventHub.ErrorOccurred event

Se produit lorsqu'une erreur survient lors d'une opération d'index.

```csharp
public event EventHandler<IndexErrorEventArgs> ErrorOccurred;
```

### Exemples

L'exemple montre comment utiliser l'événement.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

// Création d'un index
Index index = new Index(indexFolder);

// S'abonner à l'événement
index.Events.ErrorOccurred += (sender, args) =>
{
    Console.WriteLine(args.Message);
};

// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);

// Recherche dans l'index
SearchResult result = index.Search(query);
```

### Voir aussi

* class [IndexErrorEventArgs](../../indexerroreventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
