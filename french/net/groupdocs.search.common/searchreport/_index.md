---
title: "SearchReport"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente des informations détaillées sur une opération de recherche."
type: docs
weight: 300
url: /fr/net/groupdocs.search.common/searchreport/
---
## SearchReport class

Représente des informations détaillées sur une opération de recherche.

```csharp
public class SearchReport
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DocumentCount](../../groupdocs.search.common/searchreport/documentcount) { get; } | Obtient le nombre de documents trouvés. |
| [EndTime](../../groupdocs.search.common/searchreport/endtime) { get; } | Obtient l'heure de fin de la recherche. |
| [ObjectQuery](../../groupdocs.search.common/searchreport/objectquery) { get; } | Obtient la requête de recherche sous forme d'objet. |
| [OccurrenceCount](../../groupdocs.search.common/searchreport/occurrencecount) { get; } | Obtient le nombre total d'occurrences trouvées. |
| [SearchDuration](../../groupdocs.search.common/searchreport/searchduration) { get; } | Obtient la durée de la recherche. |
| [SearchOptions](../../groupdocs.search.common/searchreport/searchoptions) { get; } | Obtient les options de recherche. |
| [StartTime](../../groupdocs.search.common/searchreport/starttime) { get; } | Obtient l'heure de début de la recherche. |
| [TextQuery](../../groupdocs.search.common/searchreport/textquery) { get; } | Obtient la requête de recherche sous forme de texte. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ToString](../../groupdocs.search.common/searchreport/tostring)() | Renvoie une String qui représente le [`SearchReport`](../searchreport) actuel. |

### Remarques

**Learn more**

* [Search reports](https://docs.groupdocs.com/display/searchnet/Search+reports)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);

// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);

// Recherche dans l'index
SearchResult result1 = index.Search("Einstein");
SearchResult result2 = index.Search("\"Theory of Relativity\"");

// Obtention des rapports de recherche
SearchReport[] reports = index.GetSearchReports();

// Impression des rapports dans la console
foreach (SearchReport report in reports)
{
    Console.WriteLine("Query: " + report.TextQuery);
    Console.WriteLine("Time: " + report.StartTime);
    Console.WriteLine("Duration: " + report.SearchDuration);
    Console.WriteLine("Documents: " + report.DocumentCount);
    Console.WriteLine("Occurrences: " + report.OccurrenceCount);
    Console.WriteLine();
}
```

### Voir aussi

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
