---
title: "DateFormat"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt ein Datumsformat dar."
type: docs
weight: 810
url: /de/net/groupdocs.search.options/dateformat/
---
## DateFormat class

Stellt ein Datumsformat dar.

```csharp
public class DateFormat
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [DateFormat](dateformat#constructor)(DateFormatElement[], string) | Initialisiert eine neue Instanz der [`DateFormat`](../dateformat)-Klasse. |
| [DateFormat](dateformat#constructor_1)(string, DateFormatElement[]) | Initialisiert eine neue Instanz der [`DateFormat`](../dateformat)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DateSeparator](../../groupdocs.search.options/dateformat/dateseparator) { get; } | Gibt das Datumstrennzeichen zurück. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [ToString](../../groupdocs.search.options/dateformat/tostring)() | Gibt einen String zurück, der das aktuelle [`DateFormat`](../dateformat) darstellt. |

### Hinweise

**Learn more**

* [Date range search](https://docs.groupdocs.com/display/searchnet/Date+range+search)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

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
// Erstelle ein Datumsformatmuster 'MM/dd/yyyy'
DateFormat dateFormat = new DateFormat(elements, "/");
options.DateFormats.Add(dateFormat);

SearchResult result = index.Search(query, options); // Search in index
```

### Siehe auch

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
