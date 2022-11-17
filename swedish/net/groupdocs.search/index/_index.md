---
title: Index
second_title: GroupDocs.Search efter .NET API Reference
description: Representerar huvudklassen för att indexera dokument och söka igenom dem.
type: docs
weight: 650
url: /sv/net/groupdocs.search/index/
---
## Index class

Representerar huvudklassen för att indexera dokument och söka igenom dem.

```csharp
public class Index : IDisposable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Index](index#constructor)() | Initierar en ny instans av[`Index`](../index) klass i minnet. |
| [Index](index#constructor_1)(IndexSettings) | Initierar en ny instans av[`Index`](../index) klass i minnet med särskilda indexinställningar. |
| [Index](index#constructor_2)(string) | Initierar en ny instans av[`Index`](../index) class. Skapar ett nytt eller öppnar ett befintligt index på disken. |
| [Index](index#constructor_3)(string, bool) | Initierar en ny instans av[`Index`](../index) class. Laddar ett befintligt index från disk if*overwriteIfExists* är`falsk`; skapar ett nytt index på disken annars. |
| [Index](index#constructor_4)(string, IndexSettings) | Initierar en ny instans av[`Index`](../index) class. Skapar ett nytt index med särskilda inställningar eller öppnar ett befintligt index på disken. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Initierar en ny instans av[`Index`](../index) class. Laddar ett befintligt index från disk if*overwriteIfExists* är`falsk` ; skapar ett nytt index på disken med särskilda indexinställningar annars. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Hämtar ordboksförrådet. |
| [Events](../../groupdocs.search/index/events) { get; } | Hämtar evenemangshubben för att prenumerera på evenemang. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Får den grundläggande informationen om indexet. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Hämtar indexinställningarna. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Hämtar indexförvarsobjektet om indexet finns i det. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Utför indexeringsoperation. Lägger till en fil eller mapp med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Utför indexeringsoperation. Lägger till filer eller mappar med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Utför indexeringsoperation. Lägger till dokument från filsystem, ström eller struktur. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Utför indexeringsoperation. Lägger till extraherade data till indexet. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Utför indexeringsoperation. Lägger till en fil eller mapp med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Utför indexeringsoperation. Lägger till filer eller mappar med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Tillämpar den angivna batchen med attributändringar på indexerade dokument utan att återindexera under uppdateringsoperationen. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Tar bort indexerade filer eller mappar från indexet. Uppdaterar sedan indexet utan raderade sökvägar. Observera att ett enskilt dokument inte kan tas bort från indexet om det lades till i indexet som en del av en mapp. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Tar bort dokument som indexerats från strömmar eller strukturer. Uppdaterar sedan indexet utan raderade dokument. |
| [Dispose](../../groupdocs.search/index/dispose)() | Frigör alla resurser som används av[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Hämtar alla attribut som är associerade med det angivna indexerade dokumentet. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Genererar HTML-formaterad text för indexerade dokument och överför den via utdataadaptern. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Genererar HTML-formaterad text för indexerade dokument och överför den via utdataadaptern. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Hämtar en array av kapslade objekt i det angivna dokumentet (för containerdokument som ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Får en uppsättning av alla indexerade dokument. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Får en rad indexerade sökvägar - dokument eller mappar. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Hämtar rapporter om indexeringsåtgärder. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Hämtar rapporter om sökoperationer. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Genererar HTML-formaterad text med markerade söktermer. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Genererar HTML-formaterad text med markerade söktermer. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Slår samman det angivna indexet till det aktuella indexet. Observera att det andra indexet inte kommer att ändras. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Slår samman index från det angivna indexförrådet till det aktuella indexet. Observera att indexen i förvaret inte kommer att ändras. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Skickar det angivna meddelandeobjektet till indexet för att utföra meddelandet. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimerar antalet indexsegment genom att slå samman dem med varandra. Denna operation förbättrar sökprestanda. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimerar antalet indexsegment genom att slå samman dem med varandra. Denna operation förbättrar sökprestanda. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Söker i index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Söker i index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Utför en omvänd bildsökning i indexet. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Söker i index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Söker i index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Fortsätter bitsökningen som påbörjades med metoden Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Fortsätter bitsökningen som påbörjades med metoden Search. |
| [Update](../../groupdocs.search/index/update#update)() | Indexerar om dokument som har ändrats eller tagits bort sedan senaste uppdateringen. Lägger till nya filer som har lagts till i de indexerade mapparna. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Indexerar om dokument som har ändrats eller tagits bort sedan senaste uppdateringen. Lägger till nya filer som har lagts till i de indexerade mapparna. |

### Anmärkningar

**Läs mer**

* [Skapa ett index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexering](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Sökande](https://docs.groupdocs.com/display/searchnet/Searching)

### Exempel

Exemplet visar en typisk användning av klassen.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

SearchResult result = index.Search(query); // Söker i index
```

### Se även

* namnutrymme [GroupDocs.Search](../../groupdocs.search)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
