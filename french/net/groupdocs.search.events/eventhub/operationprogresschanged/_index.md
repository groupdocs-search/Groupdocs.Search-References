---
title: "OperationProgressChanged"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Se produit lorsque la progression de l'indexation ou de la mise à jour change."
type: docs
weight: 50
url: /fr/net/groupdocs.search.events/eventhub/operationprogresschanged/
---
## EventHub.OperationProgressChanged event

Se produit lorsque la progression de l'indexation ou de la mise à jour change.

```csharp
public event EventHandler<OperationProgressEventArgs> OperationProgressChanged;
```

### Exemples

L'exemple montre comment utiliser l'événement.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// S'abonner à l'événement
index.Events.OperationProgressChanged += (sender, args) =>
{
    Console.WriteLine("Last processed: " + args.LastDocumentPath);
    Console.WriteLine("Result: " + args.LastDocumentStatus);
    Console.WriteLine("Processed documents: " + args.TotalDocuments);
    Console.WriteLine("Progress percentage: " + args.ProgressPercentage);
};

// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);
```

### Voir aussi

* class [OperationProgressEventArgs](../../operationprogresseventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
