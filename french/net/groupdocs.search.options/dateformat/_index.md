---
title: "DateFormat"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un format de date."
type: docs
weight: 810
url: /fr/net/groupdocs.search.options/dateformat/
---
## DateFormat class

Représente un format de date.

```csharp
public class DateFormat
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DateFormat](dateformat#constructor)(DateFormatElement[], string) | Initialise une nouvelle instance de la classe [`DateFormat`](../dateformat). |
| [DateFormat](dateformat#constructor_1)(string, DateFormatElement[]) | Initialise une nouvelle instance de la classe [`DateFormat`](../dateformat). |

## Propriétés

| Nom | Description |
| --- | --- |
| [DateSeparator](../../groupdocs.search.options/dateformat/dateseparator) { get; } | Obtient le séparateur de date. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ToString](../../groupdocs.search.options/dateformat/tostring)() | Renvoie une chaîne qui représente le [`DateFormat`](../dateformat) actuel. |

### Remarques

**Learn more**

* [Date range search](https://docs.groupdocs.com/display/searchnet/Date+range+search)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "daterange(2017-01-01 ~~ 2019-12-31)";

Index index = new Index(indexFolder); // Creating an index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.DateFormats.Clear(); // Removing default date formats
DateFormatElement[] elements = new DateFormatElement[]
{
    DateFormatElement.MonthTwoDigits,
    DateFormatElement.DateSeparator,
    DateFormatElement.DayOfMonthTwoDigits,
    DateFormatElement.DateSeparator,
    DateFormatElement.YearFourDigits,
};
// Création d'un modèle de format de date 'MM/dd/yyyy'
DateFormat dateFormat = new DateFormat(elements, "/");
options.DateFormats.Add(dateFormat);

SearchResult result = index.Search(query, options); // Search in index
```

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
