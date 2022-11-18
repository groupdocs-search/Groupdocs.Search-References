---
title: SearchQuery
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta una query di ricerca sotto forma di oggetto.
type: docs
weight: 1200
url: /it/net/groupdocs.search/searchquery/
---
## SearchQuery class

Rappresenta una query di ricerca sotto forma di oggetto.

```csharp
public abstract class SearchQuery
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Ottiene il numero di query secondarie. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Ottiene il nome del campo. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Ottiene la prima query figlio. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Ottiene o imposta le opzioni di ricerca di questa query di ricerca. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Ottiene la seconda query figlio. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Crea una query per intervallo di date. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Aggiunge un campo alla query specificata. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Crea una query invertita che troverà i documenti rimanenti in un indice rispetto a quelli che verranno trovati per la query originale. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Crea una query di intervallo numerico. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Crea una query combinata che troverà tutti i documenti che verranno trovati almeno per una delle query originali. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Crea una query di ricerca per frase. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Crea una query di espressione regolare. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Crea una query di espressione regolare. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Crea un carattere jolly per la ricerca della frase. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Crea un carattere jolly per la ricerca della frase. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Crea una query modello di parola. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Crea una semplice query di parole. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Ottiene una query figlio da un indice. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Restituisce aString che rappresenta la corrente[`SearchQuery`](../searchquery) istanza. |

### Osservazioni

**Scopri di più**

* [Ricerca](https://docs.groupdocs.com/display/searchnet/Searching)
* [Interrogazioni in forma di testo e oggetto](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nidificazione delle query di ricerca sotto forma di oggetto](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Esempi

L'esempio mostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

// Creazione di una sottoquery della ricerca per intervallo di date
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Creazione di una sottoquery di caratteri jolly con numero di parole mancanti da 0 a 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Creazione di una sottoquery di una parola semplice
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Impostazione delle opzioni di ricerca solo per la sottoquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combina le sottoquery in un'unica query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Creazione di un oggetto delle opzioni di ricerca con una maggiore capacità di occorrenze trovate
SearchOptions options = new SearchOptions(); // Opzioni generali di ricerca
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Ricerca
```

### Guarda anche

* spazio dei nomi [GroupDocs.Search](../../groupdocs.search)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
