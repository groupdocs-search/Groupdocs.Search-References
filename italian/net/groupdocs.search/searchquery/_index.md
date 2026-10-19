---
title: "SearchQuery"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta una query di ricerca in forma di oggetto."
type: docs
weight: 1580
url: /it/net/groupdocs.search/searchquery/
---
## SearchQuery class

Rappresenta una query di ricerca in forma di oggetto.

```csharp
public abstract class SearchQuery
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Ottiene il numero di query figlie. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Ottiene il nome del campo. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Ottiene la prima query figlia. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Ottiene o imposta le opzioni di ricerca di questa query di ricerca. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Ottiene la seconda query figlia. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale. |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Crea una query di intervallo di date. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Aggiunge un campo alla query specificata. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Crea una query invertita che troverà i documenti rimanenti in un indice rispetto a quelli che saranno trovati per la query originale. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Crea una query di intervallo numerico. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | Crea una query combinata che troverà tutti i documenti che saranno trovati almeno per una delle query originali. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | Crea una query combinata che troverà tutti i documenti che saranno trovati almeno per una delle query originali. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Crea una query di ricerca per frase. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Crea una query di espressione regolare. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Crea una query di espressione regolare. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Crea un carattere jolly per la ricerca di frase. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Crea un carattere jolly per la ricerca di frase. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Crea una query di modello di parola. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Crea una query di parola semplice. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Ottiene una query figlia per indice. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Restituisce una String che rappresenta l'istanza corrente di [`SearchQuery`](../searchquery). |

### Osservazioni

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Creazione di sottoquery di ricerca per intervallo di date
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Creazione di sottoquery di carattere jolly con numero di parole mancanti da 0 a 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Creazione di sottoquery di parola semplice
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combinazione di sottoquery in una singola query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Creazione di oggetto opzioni di ricerca con capacità aumentata delle occorrenze trovate
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Vedi anche

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
