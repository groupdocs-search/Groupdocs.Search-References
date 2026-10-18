---
title: "DateFormats"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Liest die Sammlung von Datumsformaten für die Datumsspanne‑Suche. Die Standard‑Datumsformate sind dd.MM.yyyy, MM/dd/yyyy und yyyyMMdd."
type: docs
weight: 30
url: /de/net/groupdocs.search.options/searchoptions/dateformats/
---
## SearchOptions.DateFormats property

Liefert die Sammlung von Datumsformaten für die Datumsspanne‑Suche. Die Standard‑Datumsformate sind 'dd.MM.yyyy', 'MM/dd/yyyy' und 'yyyy-MM-dd'.

```csharp
public DateFormatCollection DateFormats { get; }
```

### Property Value

Die Sammlung von Datumsformaten für die Datumsspanne‑Suche.

### Beispiele

Das Beispiel zeigt, wie die Datumsformate für die Suche festgelegt werden.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating an index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.DateFormats.Clear(); // Removing default date formats
DateFormatElement[] elements = new DateFormatElement[]
{
    DateFormatElement.MonthTwoDigits,
    DateFormatElement.DayOfMonthTwoDigits,
    DateFormatElement.YearFourDigits,
};
// Erstelle ein Datumsformatmuster 'MM/dd/yyyy'
DateFormat dateFormat = new DateFormat(elements, "/");
options.DateFormats.Add(dateFormat);

SearchResult result = index.Search(query, options); // Search in index
```

### Siehe auch

* class [DateFormatCollection](../../dateformatcollection)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
