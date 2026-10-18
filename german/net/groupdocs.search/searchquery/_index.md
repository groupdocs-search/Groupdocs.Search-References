---
title: "SearchQuery"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt eine Suchanfrage in Objektform dar."
type: docs
weight: 1580
url: /de/net/groupdocs.search/searchquery/
---
## SearchQuery class

Stellt eine Suchanfrage in Objektform dar.

```csharp
public abstract class SearchQuery
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Ruft die Anzahl der Unterabfragen ab. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Ermittelt den Feldnamen. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Ruft die erste Unterabfrage ab. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Ruft die Suchoptionen dieser Suchabfrage ab oder legt sie fest. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Ruft die zweite Unterabfrage ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden. |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Erstellt eine Datumsbereichsabfrage. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Fügt ein Feld zur angegebenen Abfrage hinzu. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Erstellt eine invertierte Abfrage, die die restlichen Dokumente in einem Index findet, im Gegensatz zu denen, die für die ursprüngliche Abfrage gefunden werden. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Erstellt eine numerische Bereichsabfrage. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Erstellt eine Phrasensuchabfrage. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Erstellt eine reguläre Ausdrucksabfrage. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Erstellt eine reguläre Ausdrucksabfrage. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Erstellt ein Platzhalterzeichen für die Phrasensuche. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Erstellt ein Platzhalterzeichen für die Phrasensuche. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Erstellt eine Wortmusterabfrage. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Erstellt eine einfache Wortabfrage. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Ruft eine Unterabfrage anhand eines Index ab. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Gibt einen String zurück, der die aktuelle [`SearchQuery`](../searchquery)-Instanz darstellt. |

### Hinweise

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Erstelle Unterabfrage der Datumsbereichssuche.
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Erstelle Unterabfrage des Platzhalters mit einer Anzahl fehlender Wörter von 0 bis 2.
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Erstelle Unterabfrage eines einfachen Wortes.
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Kombiniere Unterabfragen zu einer Abfrage.
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Erstelle Suchoptionsobjekt mit erhöhter Kapazität gefundener Vorkommen.
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Siehe auch

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
