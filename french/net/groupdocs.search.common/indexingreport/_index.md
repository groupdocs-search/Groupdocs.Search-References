---
title: "IndexingReport"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente des informations détaillées sur une opération d'indexation."
type: docs
weight: 250
url: /fr/net/groupdocs.search.common/indexingreport/
---
## IndexingReport class

Représente des informations détaillées sur une opération d'indexation.

```csharp
public class IndexingReport
```

## Propriétés

| Nom | Description |
| --- | --- |
| [EndTime](../../groupdocs.search.common/indexingreport/endtime) { get; } | Obtient l'heure de fin de l'indexation. |
| [Errors](../../groupdocs.search.common/indexingreport/errors) { get; } | Obtient la liste des erreurs. |
| [IndexedDocuments](../../groupdocs.search.common/indexingreport/indexeddocuments) { get; } | Obtient la liste des documents indexés. |
| [IndexedDocumentsSize](../../groupdocs.search.common/indexingreport/indexeddocumentssize) { get; } | Obtient la longueur totale des documents indexés en Mo. |
| [IndexingTime](../../groupdocs.search.common/indexingreport/indexingtime) { get; } | Obtient la durée d'indexation. |
| [RemovedDocuments](../../groupdocs.search.common/indexingreport/removeddocuments) { get; } | Obtient la liste des documents retirés de l'index. |
| [SegmentCount](../../groupdocs.search.common/indexingreport/segmentcount) { get; } | Obtient le nombre de segments d'index. |
| [StartTime](../../groupdocs.search.common/indexingreport/starttime) { get; } | Obtient l'heure de début de l'indexation. |
| [TotalDocumentsInIndex](../../groupdocs.search.common/indexingreport/totaldocumentsinindex) { get; } | Obtient le nombre total de documents dans l'index. |
| [TotalIndexSize](../../groupdocs.search.common/indexingreport/totalindexsize) { get; } | Obtient la taille totale de l'index en octets. |
| [TotalTermCount](../../groupdocs.search.common/indexingreport/totaltermcount) { get; } | Obtient le nombre total de termes dans l'index. |
| [UpdatedDocuments](../../groupdocs.search.common/indexingreport/updateddocuments) { get; } | Obtient la liste des documents mis à jour. |

### Remarques

**Learn more**

* [Indexing reports](https://docs.groupdocs.com/display/searchnet/Indexing+reports)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";

// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);

// Indexation des documents
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// Obtention des rapports d'indexation
IndexingReport[] reports = index.GetIndexingReports();

// Impression des rapports dans la console
foreach (IndexingReport report in reports)
{
    Console.WriteLine("Time: " + report.StartTime);
    Console.WriteLine("Duration: " + report.IndexingTime);
    Console.WriteLine("Documents total: " + report.TotalDocumentsInIndex);
    Console.WriteLine("Terms total: " + report.TotalTermCount);
    Console.WriteLine("Indexed documents size (MB): " + report.IndexedDocumentsSize);
    Console.WriteLine("Index size (MB): " + (report.TotalIndexSize / 1024.0 / 1024.0));
    Console.WriteLine();
}
```

### Voir aussi

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
