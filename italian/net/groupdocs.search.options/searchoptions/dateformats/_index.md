---
title: "DateFormats"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Ottiene la raccolta di formati data per la ricerca per intervallo di date. I formati data predefiniti sono dd.MM.yyyy MM/dd/yyyy e yyyyMMdd."
type: docs
weight: 30
url: /it/net/groupdocs.search.options/searchoptions/dateformats/
---
## SearchOptions.DateFormats property

Restituisce la raccolta di formati di data per la ricerca per intervallo di date. I formati di data predefiniti sono 'dd.MM.yyyy', 'MM/dd/yyyy' e 'yyyy-MM-dd'.

```csharp
public DateFormatCollection DateFormats { get; }
```

### Property Value

La raccolta di formati data per la ricerca per intervallo di date.

### Esempi

L'esempio dimostra come impostare i formati data per la ricerca.

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
// Creazione di un pattern di formato data 'MM/dd/yyyy'
DateFormat dateFormat = new DateFormat(elements, "/");
options.DateFormats.Add(dateFormat);

SearchResult result = index.Search(query, options); // Search in index
```

### Vedi anche

* class [DateFormatCollection](../../dateformatcollection)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
