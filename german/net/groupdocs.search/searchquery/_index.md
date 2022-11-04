---
title: SearchQuery
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Stellt eine Suchanfrage in Objektform dar.
type: docs
weight: 1200
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
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Ruft die Anzahl der untergeordneten Abfragen ab. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Ruft den Feldnamen ab. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Ruft die erste untergeordnete Abfrage ab. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Ruft die Suchoptionen dieser Suchanfrage ab oder setzt sie. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Ruft die zweite untergeordnete Abfrage ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Erstellt eine Datumsbereichsabfrage. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Fügt der angegebenen Abfrage ein Feld hinzu. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Erstellt eine invertierte Abfrage, die die restlichen Dokumente in einem Index gegen diejenigen findet, die für die ursprüngliche Abfrage gefunden werden. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Erstellt eine numerische Bereichsabfrage. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Erstellt eine Wortgruppensuchabfrage. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Erstellt eine Abfrage mit regulären Ausdrücken. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Erstellt eine Abfrage mit regulären Ausdrücken. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Erstellt einen Platzhalter für die Phrasensuche. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Erstellt einen Platzhalter für die Phrasensuche. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Erstellt eine Wortmusterabfrage. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Erstellt eine einfache Wortabfrage. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Ruft eine untergeordnete Abfrage durch einen Index ab. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Gibt a zurückString das repräsentiert den Strom[`SearchQuery`](../searchquery) Instanz. |

### Bemerkungen

**Mehr erfahren**

* [Suchen](https://docs.groupdocs.com/display/searchnet/Searching)
* [Abfragen in Text- und Objektform](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Verschachtelung von Suchanfragen in Objektform](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

// Unterabfrage der Datumsbereichssuche erstellen
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Erstellen einer Unterabfrage des Platzhalters mit der Anzahl der fehlenden Wörter von 0 bis 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Unterabfrage eines einfachen Wortes erstellen
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Suchoptionen nur für Unterabfrage 3 setzen
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Kombinieren von Unterabfragen zu einer Abfrage
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Suchoptionsobjekt mit erhöhter Kapazität gefundener Vorkommen erstellen
SearchOptions options = new SearchOptions(); // Allgemeine Suchoptionen
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Suchen
```

### Siehe auch

* namensraum [GroupDocs.Search](../../groupdocs.search)
* Montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
