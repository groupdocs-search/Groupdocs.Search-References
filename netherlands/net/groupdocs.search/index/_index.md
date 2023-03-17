---
title: Index
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Vertegenwoordigt de hoofdklasse voor het indexeren van documenten en het doorzoeken ervan.
type: docs
weight: 680
url: /nl/net/groupdocs.search/index/
---
## Index class

Vertegenwoordigt de hoofdklasse voor het indexeren van documenten en het doorzoeken ervan.

```csharp
public class Index : IDisposable
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Index](index#constructor)() | Initialiseert een nieuw exemplaar van het[`Index`](../index) klasse in het geheugen. |
| [Index](index#constructor_1)(IndexSettings) | Initialiseert een nieuw exemplaar van het[`Index`](../index) klasse in het geheugen met bepaalde indexinstellingen. |
| [Index](index#constructor_2)(string) | Initialiseert een nieuw exemplaar van het[`Index`](../index) class. Maakt een nieuwe of opent een bestaande index op schijf. |
| [Index](index#constructor_3)(string, bool) | Initialiseert een nieuw exemplaar van het[`Index`](../index) class. Laadt een bestaande index van schijf als*overwriteIfExists* is`vals`; maakt anders een nieuwe index op schijf. |
| [Index](index#constructor_4)(string, IndexSettings) | Initialiseert een nieuw exemplaar van het[`Index`](../index) class. Maakt een nieuwe index aan met specifieke instellingen of opent een bestaande index op schijf. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Initialiseert een nieuw exemplaar van het[`Index`](../index) class. Laadt een bestaande index van schijf als*overwriteIfExists* is`vals` ; maakt een nieuwe index op schijf met anders bepaalde indexinstellingen. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Haalt de woordenboekrepository op. |
| [Events](../../groupdocs.search/index/events) { get; } | Haalt de Event Hub op voor het abonneren op events. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Krijgt de basisinformatie over de index. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Haalt de indexinstellingen op. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Haalt het indexrepository-object op als de index erin is opgenomen. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Voert indexering uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Voert indexering uit. Voegt bestanden of mappen toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Voert indexering uit. Voegt documenten toe vanuit bestandssysteem, stream of structuur. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Voert indexering uit. Voegt de geëxtraheerde gegevens toe aan de index. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Voert indexering uit. Voegt een bestand of map toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Voert indexering uit. Voegt bestanden of mappen toe via een absoluut of relatief pad. Documenten uit alle submappen worden geïndexeerd. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Past de opgegeven reeks kenmerkwijzigingen toe op geïndexeerde documenten zonder opnieuw te indexeren tijdens de updatebewerking. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Verwijdert geïndexeerde bestanden of mappen uit de index. Werkt vervolgens de index bij zonder verwijderde paden. Houd er rekening mee dat een afzonderlijk document niet uit de index kan worden verwijderd als het aan de index is toegevoegd als onderdeel van een map. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Verwijdert documenten die zijn geïndexeerd uit streams of structuren. Werkt vervolgens de index bij zonder verwijderde documenten. |
| [Dispose](../../groupdocs.search/index/dispose)() | Geeft alle bronnen vrij die worden gebruikt door de[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Haalt alle kenmerken op die zijn gekoppeld aan het opgegeven geïndexeerde document. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Genereert HTML-geformatteerde tekst voor geïndexeerd document en draagt deze over via de uitvoeradapter. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Genereert HTML-geformatteerde tekst voor geïndexeerd document en draagt deze over via de uitvoeradapter. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Haalt een reeks geneste items op van het opgegeven document (voor containerdocumenten zoals ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Krijgt een array van alle geïndexeerde documenten. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Krijgt een reeks geïndexeerde paden - documenten of mappen. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Krijgt de rapporten over indexeringsbewerkingen. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Krijgt de rapporten over zoekacties. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Genereert HTML-geformatteerde tekst met gemarkeerde gevonden termen. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Voegt de opgegeven index samen met de huidige index. Merk op dat de andere index niet wordt gewijzigd. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Voegt indexen van de gespecificeerde indexrepository samen in de huidige index. Houd er rekening mee dat indexen in de repository niet worden gewijzigd. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Geeft het opgegeven meldingsobject door aan de index om de melding uit te voeren. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Minimaliseert het aantal indexsegmenten door ze met elkaar samen te voegen. Deze bewerking verbetert de zoekprestaties. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Minimaliseert het aantal indexsegmenten door ze met elkaar samen te voegen. Deze bewerking verbetert de zoekprestaties. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Zoekopdrachten in index. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Zoekopdrachten in index. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Voert een reverse image search uit in de index. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Zoekopdrachten in index. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Zoekopdrachten in index. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Vervolgt het zoeken naar stukken dat is gestart met de methode Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Vervolgt het zoeken naar stukken dat is gestart met de methode Search. |
| [Update](../../groupdocs.search/index/update#update)() | Herindexeert documenten die zijn gewijzigd of verwijderd sinds de laatste update. Voegt nieuwe bestanden toe die zijn toegevoegd aan de geïndexeerde mappen. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Herindexeert documenten die zijn gewijzigd of verwijderd sinds de laatste update. Voegt nieuwe bestanden toe die zijn toegevoegd aan de geïndexeerde mappen. |

### Opmerkingen

**Kom meer te weten**

* [Een index maken](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexeren](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Zoeken](https://docs.groupdocs.com/display/searchnet/Searching)

### Voorbeelden

Het voorbeeld demonstreert een typisch gebruik van de klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

SearchResult result = index.Search(query); // Zoeken in index
```

### Zie ook

* naamruimte [GroupDocs.Search](../../groupdocs.search)
* montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
