---
title: DateFormat
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta un formato data.
type: docs
weight: 740
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
| [DateFormat](dateformat#constructor)(DateFormatElement[], string) | Inizializza una nuova istanza di[`DateFormat`](../dateformat) classe. |
| [DateFormat](dateformat#constructor_1)(string, DateFormatElement[]) | Inizializza una nuova istanza di[`DateFormat`](../dateformat) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DateSeparator](../../groupdocs.search.options/dateformat/dateseparator) { get; } | Ottiene il separatore di data. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ToString](../../groupdocs.search.options/dateformat/tostring)() | Restituisce aString che rappresenta la corrente[`DateFormat`](../dateformat) . |

### Osservazioni

**Scopri di più**

* [Ricerca per intervallo di date](https://docs.groupdocs.com/display/searchnet/Date+range+search)

### Esempi

L'esempio mostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "daterange(2017-01-01 ~~ 2019-12-31)";

Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

SearchOptions options = new SearchOptions();
options.DateFormats.Clear(); // Rimozione dei formati di data predefiniti
DateFormatElement[] elements = new DateFormatElement[]
{
    DateFormatElement.MonthTwoDigits,
    DateFormatElement.DateSeparator,
    DateFormatElement.DayOfMonthTwoDigits,
    DateFormatElement.DateSeparator,
    DateFormatElement.YearFourDigits,
};
// Creazione di un modello di formato data 'MM/gg/aaaa'
DateFormat dateFormat = new DateFormat(elements, "/");
options.DateFormats.Add(dateFormat);

SearchResult result = index.Search(query, options); // Cerca nell'indice
```

### Guarda anche

* spazio dei nomi [GroupDocs.Search.Options](../../groupdocs.search.options)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->