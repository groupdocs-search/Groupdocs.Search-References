---
title: SearchReport
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Vertegenwoordigt gedetailleerde informatie over een zoekopdracht.
type: docs
weight: 290
url: /nl/net/groupdocs.search.common/searchreport/
---
## SearchReport class

Vertegenwoordigt gedetailleerde informatie over een zoekopdracht.

```csharp
public class SearchReport
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [DocumentCount](../../groupdocs.search.common/searchreport/documentcount) { get; } | Haalt het aantal gevonden documenten op. |
| [EndTime](../../groupdocs.search.common/searchreport/endtime) { get; } | Haalt de eindtijd van de zoekopdracht op. |
| [ObjectQuery](../../groupdocs.search.common/searchreport/objectquery) { get; } | Haalt de zoekopdracht op in objectvorm. |
| [OccurrenceCount](../../groupdocs.search.common/searchreport/occurrencecount) { get; } | Haalt het totale aantal gevonden exemplaren op. |
| [SearchDuration](../../groupdocs.search.common/searchreport/searchduration) { get; } | Haalt de zoekduur op. |
| [SearchOptions](../../groupdocs.search.common/searchreport/searchoptions) { get; } | Krijgt de zoekopties. |
| [StartTime](../../groupdocs.search.common/searchreport/starttime) { get; } | Krijgt de starttijd van de zoekopdracht. |
| [TextQuery](../../groupdocs.search.common/searchreport/textquery) { get; } | Krijgt de zoekopdracht in tekstvorm. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [ToString](../../groupdocs.search.common/searchreport/tostring)() | Geeft als resultaat eenString dat vertegenwoordigt de stroom[`SearchReport`](../searchreport) . |

### Opmerkingen

**Kom meer te weten**

* [Zoek rapporten](https://docs.groupdocs.com/display/searchnet/Search+reports)

### Voorbeelden

Het voorbeeld demonstreert een typisch gebruik van de klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Een index maken in de opgegeven map
Index index = new Index(indexFolder);

// Documenten uit de opgegeven map indexeren
index.Add(documentsFolder);

// Zoeken in index
SearchResult result1 = index.Search("Einstein");
SearchResult result2 = index.Search("\"Theory of Relativity\"");

// Zoekrapporten ophalen
SearchReport[] reports = index.GetSearchReports();

// Afdrukken van rapporten naar de console
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

### Zie ook

* naamruimte [GroupDocs.Search.Common](../../groupdocs.search.common)
* montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->