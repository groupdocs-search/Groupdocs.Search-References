---
title: SearchQuery
second_title: GroupDocs.Search efter .NET API Reference
description: Representerar en sökfråga i objektform.
type: docs
weight: 1200
url: /sv/net/groupdocs.search/searchquery/
---
## SearchQuery class

Representerar en sökfråga i objektform.

```csharp
public abstract class SearchQuery
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Hämtar antalet underordnade frågor. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Hämtar fältnamnet. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Får den första underordnade frågan. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Hämtar eller ställer in sökalternativen för denna sökfråga. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Hämtar den andra underordnade frågan. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Skapar en kombinerad fråga som endast hittar dokument som kommer att hittas för varje ursprunglig fråga. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Skapar en datumintervallfråga. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Lägger till ett fält i den angivna frågan. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Skapar en inverterad fråga som hittar resten av dokumenten i ett index mot de som kommer att hittas för den ursprungliga frågan. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Skapar en numerisk intervallfråga. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Skapar en kombinerad fråga som hittar alla dokument som kommer att hittas för åtminstone en av de ursprungliga frågorna. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Skapar en frassökning. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Skapar en reguljär uttrycksfråga. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Skapar en reguljär uttrycksfråga. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Skapar ett jokertecken för frassökningen. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Skapar ett jokertecken för frassökningen. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Skapar en ordmönsterfråga. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Skapar en enkel ordfråga. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Får en underordnad fråga med ett index. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Returnerar enString som representerar strömmen[`SearchQuery`](../searchquery) instans. |

### Anmärkningar

**Läs mer**

* [Sökande](https://docs.groupdocs.com/display/searchnet/Searching)
* [Frågor i text- och objektform](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Kapsling av sökfrågor i objektform](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Exempel

Exemplet visar en typisk användning av klassen.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

// Skapar underfråga till datumintervallsökning
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Skapar underfråga av jokertecken med antalet missade ord från 0 till 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Skapar underfråga av enkelt ord
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Ställ in sökalternativ endast för delfråga 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Kombinera delfrågor till en fråga
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Skapar sökalternativsobjekt med ökad kapacitet för hittade förekomster
SearchOptions options = new SearchOptions(); // Övergripande sökalternativ
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Söker
```

### Se även

* namnutrymme [GroupDocs.Search](../../groupdocs.search)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
