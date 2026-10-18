---
title: "OperationFinished"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Se produit lorsqu'une opération d'index est terminée."
type: docs
weight: 40
url: /fr/net/groupdocs.search.events/eventhub/operationfinished/
---
## EventHub.OperationFinished event

Se produit lorsqu'une opération d'index est terminée.

```csharp
public event EventHandler<OperationFinishedEventArgs> OperationFinished;
```

### Exemples

L'exemple montre comment utiliser l'événement.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// S'abonner à l'événement
index.Events.OperationFinished += (sender, args) =>
{
    Console.WriteLine("Operation finished: " + args.OperationType);
    Console.WriteLine("Message: " + args.Message);
    Console.WriteLine("Index folder: " + args.IndexFolder);
    Console.WriteLine("Time: " + args.Time);
};

// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);
```

### Voir aussi

* class [OperationFinishedEventArgs](../../operationfinishedeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
