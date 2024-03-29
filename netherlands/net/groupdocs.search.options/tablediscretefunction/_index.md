---
title: TableDiscreteFunction
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Vertegenwoordigt het fuzzyzoekalgoritme dat overeenkomsten bevat tussen woordlengtes en het aantal toegestane fouten. Dit algoritme kan worden gespecificeerd door een tabel met uitvoerwaarden of door een stapfunctie.
type: docs
weight: 1090
url: /nl/net/groupdocs.search.options/tablediscretefunction/
---
## TableDiscreteFunction class

Vertegenwoordigt het fuzzy-zoekalgoritme dat overeenkomsten bevat tussen woordlengtes en het aantal toegestane fouten. Dit algoritme kan worden gespecificeerd door een tabel met uitvoerwaarden of door een stapfunctie.

```csharp
public class TableDiscreteFunction : FuzzyAlgorithm
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [TableDiscreteFunction](tablediscretefunction#constructor_1)(int, int[]) | Initialiseert een nieuw exemplaar van het[`TableDiscreteFunction`](../tablediscretefunction) klasse. |
| [TableDiscreteFunction](tablediscretefunction#constructor)(int, params Step[]) | Initialiseert een nieuw exemplaar van het[`TableDiscreteFunction`](../tablediscretefunction) klasse. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/tablediscretefunction/getmaxmistakecount)(int) | Krijgt een maximaal toegestaan aantal fouten voor de gespecificeerde termijnlengte. |
| override [GetSimilarityLevel](../../groupdocs.search.options/tablediscretefunction/getsimilaritylevel)(int) | Krijgt een overeenkomstniveau voor de gespecificeerde termijnlengte. |

### Opmerkingen

**Kom meer te weten**

* [Vage zoektocht](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)

### Voorbeelden

Het voorbeeld demonstreert een typisch gebruik van de klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Een index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // De fuzzy search inschakelen
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3)); // Het algoritme voor fuzzy zoeken maken
// Deze functie specificeert 1 als het maximale aantal fouten voor woorden van 1 tot 4 tekens.
// Het specificeert 2 als het maximale aantal fouten voor woorden van 5 tot 7 tekens.
// Het specificeert 3 als het maximale aantal fouten voor woorden van 8 en meer tekens.

SearchResult result = index.Search(query, options); // Zoeken in index
```

### Zie ook

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* naamruimte [GroupDocs.Search.Options](../../groupdocs.search.options)
* montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
