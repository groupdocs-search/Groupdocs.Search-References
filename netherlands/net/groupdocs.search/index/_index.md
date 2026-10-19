---
title: "Index"
second_title: "GroupDocs.Search voor .NET API-referentie"
description: "Stelt de hoofdklasse voor het indexeren van documenten en zoeken daarin."
type: docs
weight: 700
url: /nl/net/groupdocs.search/index/
---
## Index class

Stelt de hoofdklasse voor het indexeren van documenten en zoeken daarin.

```csharp
public class Index : IDisposable
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [Index](index#constructor)() | Initialiseert een nieuw exemplaar van de [`Index`](../index) klasse in het geheugen. |
| [Index](index#constructor_1)(IndexSettings) | Initialiseert een nieuw exemplaar van de [`Index`](../index) klasse in het geheugen met specifieke indexinstellingen. |
| [Index](index#constructor_2)(string) | Initialiseert een nieuw exemplaar van de [`Index`](../index) klasse. Maakt een nieuwe index aan of opent een bestaande index op schijf. |
| [Index](index#constructor_3)(string, bool) | Initialiseert een nieuw exemplaar van de [`Index`](../index) klasse. Laadt een bestaande index van schijf als *overwriteIfExists* `false` is; maakt anders een nieuwe index op schijf aan. |
| [Index](index#constructor_4)(string, IndexSettings) | Initialiseert een nieuw exemplaar van de [`Index`](../index) klasse. Maakt een nieuwe index met specifieke instellingen of opent een bestaande index op schijf. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Initialiseert een nieuw exemplaar van de [`Index`](../index) klasse. Laadt een bestaande index van schijf als *overwriteIfExists* `false` is; maakt anders een nieuwe index op schijf met specifieke indexinstellingen. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Haalt de woordenboekrepository op. |
| [Events](../../groupdocs.search/index/events) { get; } | Haalt de event-hub op voor het abonneren op gebeurtenissen. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Haalt de basisinformatie over de index op. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Haalt de indexinstellingen op. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Haalt het indexrepository‑object op als de index erin is opgenomen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Laadt de volledige index in het geheugen. Wijzigingen aan de index worden niet automatisch opgeslagen in de oorspronkelijke map. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Laadt de volledige index in het geheugen. Wijzigingen aan de index worden niet automatisch opgeslagen in de oorspronkelijke map. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Voert een indexeerbewerking uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Voert een indexeerbewerking uit. Voegt bestanden of mappen toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Voert een indexeerbewerking uit. Voegt documenten toe vanuit het bestandssysteem, een stream of een structuur. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Voert een indexeerbewerking uit. Voegt de geëxtraheerde gegevens toe aan de index. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Voert een indexeerbewerking uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Voert een indexeerbewerking uit. Voegt bestanden of mappen toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Past de opgegeven batch attribuutwijzigingen toe op geïndexeerde documenten zonder opnieuw te indexeren tijdens de update‑bewerking. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Controleert de index op beschadigde segmentbestanden op de schijf. De methode herstelt de indexfunctionaliteit bij beschadigde segmenten als *fixIndexFunctionality* `true` is; herstelt anders niet. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Verwijdert geïndexeerde bestanden of mappen uit de index. Werk vervolgens de index bij zonder de verwijderde paden. Merk op dat een individueel document niet uit de index kan worden verwijderd als het als onderdeel van een map aan de index is toegevoegd. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Verwijdert documenten die uit streams of structuren zijn geïndexeerd. Werk vervolgens de index bij zonder de verwijderde documenten. |
| [Dispose](../../groupdocs.search/index/dispose)() | Geeft alle bronnen vrij die door de [`Index`](../index) worden gebruikt. |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Haalt alle attributen op die gekoppeld zijn aan het opgegeven geïndexeerde document. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Genereert de tekst van een geïndexeerd document en geeft deze door aan een output‑adapter. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Genereert HTML‑geformatteerde tekst voor een geïndexeerd document en stuurt deze door via de output‑adapter. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Haalt een geïndexeerd document op via de documentsleutel. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Haalt een array op van geneste items van het opgegeven document (voor container‑documenten zoals ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Haalt een array op van alle geïndexeerde documenten. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Haalt een array op van geïndexeerde paden – documenten of mappen. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Haalt de rapporten over indexeerbewerkingen op. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Haalt de rapporten over zoekbewerkingen op. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Voegt de opgegeven index samen met de huidige index. Merk op dat de andere index niet wordt gewijzigd. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Voegt indexen uit de opgegeven indexrepository samen met de huidige index. Merk op dat indexen in de repository niet worden gewijzigd. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Geeft het opgegeven meldingsobject door aan de index om de melding uit te voeren. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimaliseert het aantal indexsegmenten door ze met elkaar te combineren. Deze bewerking verbetert de zoekprestaties. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimaliseert het aantal indexsegmenten door ze met elkaar te combineren. Deze bewerking verbetert de zoekprestaties. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Slaat de in-memory index op naar schijf. Slaat ook de reguliere index op in een andere map. Wijzigt de instellingen van deze index niet. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Zoekt in de index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Zoekt in de index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Voert een omgekeerde afbeeldingzoekopdracht uit in de index. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Zoekt in de index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Zoekt in de index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Vervolg de chunk-zoekopdracht gestart met de methode Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Vervolg de chunk-zoekopdracht gestart met de methode Search. |
| [Update](../../groupdocs.search/index/update#update)() | Indexeert documenten die sinds de laatste update zijn gewijzigd of verwijderd opnieuw. Voegt nieuwe bestanden toe die aan de geïndexeerde mappen zijn toegevoegd. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Indexeert documenten die sinds de laatste update zijn gewijzigd of verwijderd opnieuw. Voegt nieuwe bestanden toe die aan de geïndexeerde mappen zijn toegevoegd. |

### Opmerkingen

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Voorbeelden

Het voorbeeld toont een typisch gebruik van de klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### Zie ook

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
