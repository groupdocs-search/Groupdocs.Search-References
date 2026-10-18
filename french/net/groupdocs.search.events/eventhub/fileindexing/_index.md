---
title: "FileIndexing"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Se produit lorsqu'un document va être indexé."
type: docs
weight: 20
url: /fr/net/groupdocs.search.events/eventhub/fileindexing/
---
## EventHub.FileIndexing event

Se produit lorsqu'un document va être indexé.

```csharp
public event EventHandler<FileIndexingEventArgs> FileIndexing;
```

### Exemples

L'exemple montre comment utiliser l'événement.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// S'abonner à l'événement
index.Events.FileIndexing += (sender, args) =>
{
    if (args.DocumentFullPath.EndsWith("Protected.pdf", StringComparison.InvariantCultureIgnoreCase))
    {
        args.AdditionalFields = new DocumentField[]
        {
            new DocumentField("Tags", "Protected")
        };
    }
    if (!args.DocumentFullPath.ToLowerInvariant().Contains("important"))
    {
        args.SkipIndexing = true;
    }
};

// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);
```

### Voir aussi

* class [FileIndexingEventArgs](../../fileindexingeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
