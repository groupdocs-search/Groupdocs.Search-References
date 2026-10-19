---
title: "SearchQuery"
second_title: "GroupDocs.Search voor .NET API-referentie"
description: "Stelt een zoekquery in objectvorm voor."
type: docs
weight: 1580
url: /nl/net/groupdocs.search/searchquery/
---
## SearchQuery class

Stelt een zoekquery in objectvorm voor.

```csharp
public abstract class SearchQuery
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Haalt het aantal onderliggende queries op. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Haalt de veldnaam op. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Haalt de eerste onderliggende query op. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Haalt of stelt de zoekopties van deze zoekquery in. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Haalt de tweede onderliggende query op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | Maakt een gecombineerde query die alleen documenten vindt die voor elke originele query gevonden worden. |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | Maakt een gecombineerde query die alleen documenten vindt die voor elke originele query gevonden worden. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Maakt een datumreeksquery aan. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Voegt een veld toe aan de opgegeven query. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Maakt een omgekeerde query die de overige documenten in een index vindt ten opzichte van diegene die voor de oorspronkelijke query worden gevonden. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Maakt een numerieke bereikquery. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | Maakt een gecombineerde query die alle documenten vindt die ten minste voor één van de oorspronkelijke queries worden gevonden. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | Maakt een gecombineerde query die alle documenten vindt die ten minste voor één van de oorspronkelijke queries worden gevonden. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Maakt een frase‑zoekquery aan. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Maakt een reguliere‑expressie‑query aan. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Maakt een reguliere‑expressie‑query aan. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Maakt een wildcard voor de frase‑zoekopdracht. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Maakt een wildcard voor de frase‑zoekopdracht. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Maakt een woordpatroon‑query aan. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Maakt een eenvoudige woordquery aan. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Haalt een onderliggende query op via een index. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Retourneert een String die de huidige [`SearchQuery`](../searchquery) instantie vertegenwoordigt. |

### Opmerkingen

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Voorbeelden

Het voorbeeld toont een typisch gebruik van de klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Subquery maken voor datumreekszoekopdracht
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Subquery maken voor wildcard met een aantal gemiste woorden van 0 tot 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Subquery maken voor eenvoudig woord
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Subqueries combineren tot één query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Zoekopties‑object maken met verhoogde capaciteit voor gevonden voorkomen.
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Zie ook

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
