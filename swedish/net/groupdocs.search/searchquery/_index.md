---
title: "SearchQuery"
second_title: "GroupDocs.Search för .NET API-referens"
description: "Representerar en sökfråga i objektform."
type: docs
weight: 1580
url: /sv/net/groupdocs.search/searchquery/
---
## SearchQuery class

Representerar en sökfråga i objektform.

```csharp
public abstract class SearchQuery
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Hämtar antalet underfrågor. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Hämtar fältnamnet. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Hämtar den första underfrågan. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Hämtar eller anger sökalternativen för denna sökfråga. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Hämtar den andra underfrågan. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | Skapar en kombinerad fråga som endast hittar dokument som hittas för varje ursprunglig fråga. |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | Skapar en kombinerad fråga som endast hittar dokument som hittas för varje ursprunglig fråga. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Skapar en datumintervallfråga. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Lägger till ett fält i den angivna frågan. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Skapar en inverterad fråga som hittar de återstående dokumenten i ett index jämfört med de som hittas för den ursprungliga frågan. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Skapar en numerisk intervallfråga. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | Skapar en kombinerad fråga som hittar alla dokument som hittas åtminstone av en av de ursprungliga frågorna. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | Skapar en kombinerad fråga som hittar alla dokument som hittas åtminstone av en av de ursprungliga frågorna. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Skapar en frasökfråga. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Skapar en reguljäruttrycksfråga. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Skapar en reguljäruttrycksfråga. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Skapar ett jokertecken för frassökning. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Skapar ett jokertecken för frassökning. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Skapar en ordmönsterfråga. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Skapar en enkel ordfråga. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Hämtar en underfråga efter ett index. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Returnerar en String som representerar den aktuella [`SearchQuery`](../searchquery)-instansen. |

### Anmärkningar

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Exempel

Exemplet visar ett typiskt användningssätt av klassen.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Skapar delfråga för datumintervallsökning.
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Skapar delfråga för jokertecken med antal saknade ord från 0 till 2.
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Skapar delfråga för enkelt ord.
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Kombinerar delfrågor till en fråga.
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Skapar sökalternativobjekt med ökad kapacitet för hittade förekomster.
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Se även

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
