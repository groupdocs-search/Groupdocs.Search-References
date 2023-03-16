---
title: SearchQuery
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Vertegenwoordigt een zoekopdracht in objectvorm.
type: docs
weight: 1240
url: /nl/net/groupdocs.search/searchquery/
---
## SearchQuery class

Vertegenwoordigt een zoekopdracht in objectvorm.

```csharp
public abstract class SearchQuery
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Haalt het aantal onderliggende query's op. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Krijgt de veldnaam. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Haalt de eerste onderliggende query op. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Haalt de zoekopties van deze zoekopdracht op of stelt deze in. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Haalt de tweede onderliggende query op. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Creëert een gecombineerde zoekopdracht die alleen documenten vindt die voor elke oorspronkelijke zoekopdracht worden gevonden. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Maakt een query voor een datumbereik. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Voegt een veld toe aan de opgegeven query. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Creëert een geïnverteerde query die de overige documenten in een index zal vinden tegen de documenten die zullen worden gevonden voor de originele query. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Maakt een query voor een numeriek bereik. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Creëert een gecombineerde zoekopdracht die alle documenten vindt die tenminste voor één van de oorspronkelijke zoekopdrachten worden gevonden. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Creëert een zoekopdracht op woordgroep. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Maakt een query voor een reguliere expressie. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Maakt een query voor een reguliere expressie. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Creëert een jokerteken voor het zoeken naar zin. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Creëert een jokerteken voor het zoeken naar zin. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Creëert een woordpatroonquery. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Creëert een eenvoudige woordquery. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Krijgt een onderliggende query door een index. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Geeft als resultaat eenString dat vertegenwoordigt de stroom[`SearchQuery`](../searchquery) instantie. |

### Opmerkingen

**Kom meer te weten**

* [Zoeken](https://docs.groupdocs.com/display/searchnet/Searching)
* [Query's in tekst- en objectvorm](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Zoekopdrachten nesten in objectvorm](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Voorbeelden

Het voorbeeld demonstreert een typisch gebruik van de klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

// Subquery maken van zoeken in datumbereik
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Subquery van wildcard maken met aantal gemiste woorden van 0 tot 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Subquery maken van een eenvoudig woord
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Zoekopties alleen instellen voor subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Subquery's combineren tot één query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Een object met zoekopties maken met een grotere capaciteit van gevonden voorvallen
SearchOptions options = new SearchOptions(); // Algemene zoekopties
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Zoeken
```

### Zie ook

* naamruimte [GroupDocs.Search](../../groupdocs.search)
* montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
