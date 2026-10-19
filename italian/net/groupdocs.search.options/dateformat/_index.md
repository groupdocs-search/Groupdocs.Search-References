---
title: "DateFormat"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un formato data."
type: docs
weight: 810
url: /it/net/groupdocs.search.options/dateformat/
---
## DateFormat class

Rappresenta un formato data.

```csharp
public class DateFormat
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DateFormat](dateformat#constructor)(DateFormatElement[], string) | Inizializza una nuova istanza della classe [`DateFormat`](../dateformat). |
| [DateFormat](dateformat#constructor_1)(string, DateFormatElement[]) | Inizializza una nuova istanza della classe [`DateFormat`](../dateformat). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DateSeparator](../../groupdocs.search.options/dateformat/dateseparator) { get; } | Ottiene il separatore di data. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ToString](../../groupdocs.search.options/dateformat/tostring)() | Restituisce una String che rappresenta l'attuale [`DateFormat`](../dateformat). |

### Osservazioni

**Learn more**

* [Date range search](https://docs.groupdocs.com/display/searchnet/Date+range+search)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

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
// Creazione di un pattern di formato data 'MM/dd/yyyy'
DateFormat dateFormat = new DateFormat(elements, "/");
options.DateFormats.Add(dateFormat);

SearchResult result = index.Search(query, options); // Search in index
```

### Vedi anche

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
