---
title: SearchPhaseCompleted
second_title: GroupDocs.Buscar referencia de API de .NET
description: Ocurre cuando se completa la fase de búsqueda.
type: docs
weight: 70
url: /es/net/groupdocs.search.events/eventhub/searchphasecompleted/
---
## EventHub.SearchPhaseCompleted event

Ocurre cuando se completa la fase de búsqueda.

```csharp
public event EventHandler<SearchPhaseEventArgs> SearchPhaseCompleted;
```

### Ejemplos

El ejemplo demuestra cómo usar el evento.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creando un índice
Index index = new Index(indexFolder);

// Indexación de documentos de la carpeta especificada
index.Add(documentsFolder);

// Suscribiendose al evento
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

### Ver también

* class [SearchPhaseEventArgs](../../searchphaseeventargs)
* class [EventHub](../../eventhub)
* espacio de nombres [GroupDocs.Search.Events](../../eventhub)
* asamblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
