---
title: "Index"
second_title: "GroupDocs.Search för .NET API-referens"
description: "Representerar huvudklassen för indexering av dokument och sökning genom dem."
type: docs
weight: 700
url: /sv/net/groupdocs.search/index/
---
## Index class

Representerar huvudklassen för indexering av dokument och sökning genom dem.

```csharp
public class Index : IDisposable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Index](index#constructor)() | Initierar en ny instans av klassen [`Index`](../index) i minnet. |
| [Index](index#constructor_1)(IndexSettings) | Initierar en ny instans av klassen [`Index`](../index) i minnet med specifika indexinställningar. |
| [Index](index#constructor_2)(string) | Initierar en ny instans av klassen [`Index`](../index). Skapar ett nytt eller öppnar ett befintligt index på disk. |
| [Index](index#constructor_3)(string, bool) | Initierar en ny instans av klassen [`Index`](../index). Laddar ett befintligt index från disk om *overwriteIfExists* är `false`; skapar annars ett nytt index på disk. |
| [Index](index#constructor_4)(string, IndexSettings) | Initierar en ny instans av klassen [`Index`](../index). Skapar ett nytt index med särskilda inställningar eller öppnar ett befintligt index på disk. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Initierar en ny instans av klassen [`Index`](../index). Laddar ett befintligt index från disk om *overwriteIfExists* är `false`; skapar annars ett nytt index på disk med särskilda indexinställningar. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Hämtar ordboksförrådet. |
| [Events](../../groupdocs.search/index/events) { get; } | Hämtar händelsehubben för att prenumerera på händelser. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Hämtar grundläggande information om indexet. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Hämtar indexinställningarna. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Hämtar indexförrådsobjektet om indexet finns i det. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Laddar hela indexet i minnet. Eventuella ändringar i indexet sparas inte automatiskt till den ursprungliga mappen. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Laddar hela indexet i minnet. Eventuella ändringar i indexet sparas inte automatiskt till den ursprungliga mappen. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Utför indexeringsoperation. Lägger till en fil eller mapp med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Utför indexeringsoperation. Lägger till filer eller mappar med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Utför indexeringsoperation. Lägger till dokument från filsystem, ström eller struktur. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Utför indexeringsoperation. Lägger till den extraherade datan i indexet. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Utför indexeringsoperation. Lägger till en fil eller mapp med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Utför indexeringsoperation. Lägger till filer eller mappar med en absolut eller relativ sökväg. Dokument från alla undermappar kommer att indexeras. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Tillämpar den angivna batchen av attributändringar på indexerade dokument utan omindexering under uppdateringsoperationen. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Kontrollerar indexet för skadade segmentfiler på disken. Metoden reparerar indexfunktionaliteten vid skadade segment om *fixIndexFunctionality* är true; reparerar annars inte. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Tar bort indexerade filer eller mappar från indexet. Uppdaterar sedan indexet utan de borttagna sökvägarna. Observera att ett enskilt dokument inte kan tas bort från indexet om det lades till som en del av en mapp. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Tar bort dokument som indexerats från strömmar eller strukturer. Uppdaterar sedan indexet utan de borttagna dokumenten. |
| [Dispose](../../groupdocs.search/index/dispose)() | Frigör alla resurser som används av [`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Hämtar alla attribut som är associerade med det angivna indexerade dokumentet. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Genererar texten för ett indexerat dokument och skickar den genom en utdataadapter. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Genererar HTML-formaterad text för ett indexerat dokument och överför den genom utdataadaptern. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Hämtar ett indexerat dokument med dokumentnyckel. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Hämtar en array av nästlade objekt i det angivna dokumentet (för container-dokument såsom ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Hämtar en array med alla indexerade dokument. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Hämtar en array av indexerade sökvägar – dokument eller mappar. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Hämtar rapporterna om indexeringsoperationer. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Hämtar rapporterna om sökoperationer. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Genererar HTML-formaterad text med markerade hittade termer. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Genererar HTML-formaterad text med markerade hittade termer. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Slår ihop det angivna indexet med det aktuella indexet. Observera att det andra indexet inte kommer att ändras. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Slår ihop index från det angivna indexförrådet med det aktuella indexet. Observera att index i förrådet inte kommer att ändras. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Skickar det angivna aviseringsobjektet till indexet för att utföra aviseringen. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimerar antalet indexsegment genom att slå ihop dem med varandra. Denna operation förbättrar sökprestanda. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimerar antalet indexsegment genom att slå ihop dem med varandra. Denna operation förbättrar sökprestanda. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Sparar det minnesbaserade indexet till disk. Sparar också det vanliga indexet till en annan mapp. Ändrar inte inställningarna för detta index. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Söker i indexet. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Söker i indexet. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Utför en omvänd bildsökning i indexet. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Söker i indexet. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Söker i indexet. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Fortsätter chunk-sökningen som startades med metoden Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Fortsätter chunk-sökningen som startades med metoden Search. |
| [Update](../../groupdocs.search/index/update#update)() | Återindexerar dokument som har ändrats eller raderats sedan senaste uppdateringen. Lägger till nya filer som har lagts till i de indexerade mapparna. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Återindexerar dokument som har ändrats eller raderats sedan senaste uppdateringen. Lägger till nya filer som har lagts till i de indexerade mapparna. |

### Anmärkningar

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Exempel

Exemplet visar ett typiskt användningssätt av klassen.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### Se även

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
