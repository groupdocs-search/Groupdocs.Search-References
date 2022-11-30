---
title: IndexRepository
second_title: GroupDocs.Search efter .NET API Reference
description: Representerar en behållare för att kombinera flera index och utföra vanliga operationer på dem.
type: docs
weight: 660
url: /sv/net/groupdocs.search/indexrepository/
---
## IndexRepository class

Representerar en behållare för att kombinera flera index och utföra vanliga operationer på dem.

```csharp
public class IndexRepository : IDisposable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [IndexRepository](indexrepository)() | Initierar en ny instans av[`IndexRepository`](../indexrepository) class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Events](../../groupdocs.search/indexrepository/events) { get; } | Hämtar evenemangshubben för att prenumerera på evenemang. |
| [Indexes](../../groupdocs.search/indexrepository/indexes) { get; } | Hämtar indexen som finns i detta[`IndexRepository`](../indexrepository) . |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository)(Index) | Lägger till ett index i indexförrådet. |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository_1)(string) | Öppnar och lägger till ett index i indexförrådet. |
| [Create](../../groupdocs.search/indexrepository/create#create)() | Skapar ett nytt index i minnet. |
| [Create](../../groupdocs.search/indexrepository/create#create_1)(IndexSettings) | Skapar ett nytt index i minnet. |
| [Create](../../groupdocs.search/indexrepository/create#create_2)(string) | Skapar ett nytt index på disken. Indexmappen kommer att rengöras innan indexet skapas. |
| [Create](../../groupdocs.search/indexrepository/create#create_3)(string, IndexSettings) | Skapar ett nytt index på disken. Indexmappen kommer att rengöras innan indexet skapas. |
| [Dispose](../../groupdocs.search/indexrepository/dispose)() | Frigör alla resurser som används av[`IndexRepository`](../indexrepository) . |
| [Search](../../groupdocs.search/indexrepository/search#search)(SearchQuery) | Söker i alla index i förvaret. |
| [Search](../../groupdocs.search/indexrepository/search#search_2)(string) | Söker i alla index i förvaret. |
| [Search](../../groupdocs.search/indexrepository/search#search_1)(SearchQuery, SearchOptions) | Söker i alla index i förvaret. |
| [Search](../../groupdocs.search/indexrepository/search#search_3)(string, SearchOptions) | Söker i alla index i förvaret. |
| [Update](../../groupdocs.search/indexrepository/update#update)() | Uppdaterar alla index i arkivet. |
| [Update](../../groupdocs.search/indexrepository/update#update_1)(UpdateOptions) | Uppdaterar alla index i arkivet. |

### Anmärkningar

**Läs mer**

* [Sök i indexförråd](https://docs.groupdocs.com/display/searchnet/Search+index+repository)

### Exempel

Exemplet visar en typisk användning av klassen.

```csharp
string indexFolder1 = @"c:\MyIndex\";
string indexFolder2 = @"c:\MyIndex\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
repository.AddToRepository(indexFolder1); // Laddar ett befintligt index
repository.AddToRepository(indexFolder2); // Laddar ett annat befintligt index

SearchResult result = repository.Search(query); // Söker i index för förvaret
```

### Se även

* namnutrymme [GroupDocs.Search](../../groupdocs.search)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->