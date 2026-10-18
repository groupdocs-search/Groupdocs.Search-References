---
title: "DateFormats"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Obtient la collection de formats de date pour la recherche de plage de dates. Les formats de date par défaut sont dd.MM.yyyy MM/dd/yyyy et yyyyMMdd."
type: docs
weight: 30
url: /fr/net/groupdocs.search.options/searchoptions/dateformats/
---
## SearchOptions.DateFormats property

Obtient la collection de formats de date pour la recherche de plage de dates. Les formats de date par défaut sont 'dd.MM.yyyy', 'MM/dd/yyyy' et 'yyyy-MM-dd'.

```csharp
public DateFormatCollection DateFormats { get; }
```

### Property Value

La collection de formats de date pour la recherche de plage de dates.

### Exemples

L'exemple montre comment définir les formats de date pour la recherche.

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
// Création d'un modèle de format de date 'MM/dd/yyyy'
DateFormat dateFormat = new DateFormat(elements, "/");
options.DateFormats.Add(dateFormat);

SearchResult result = index.Search(query, options); // Search in index
```

### Voir aussi

* class [DateFormatCollection](../../dateformatcollection)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
