---
title: "IndexSettings"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta le impostazioni dell'indice che consentono di personalizzare le operazioni di indicizzazione."
type: docs
weight: 720
url: /it/net/groupdocs.search/indexsettings/
---
## IndexSettings class

Rappresenta le impostazioni dell'indice che consentono di personalizzare le operazioni di indicizzazione.

```csharp
public class IndexSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [IndexSettings](indexsettings)() | Inizializza una nuova istanza della classe [`IndexSettings`](../indexsettings). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CustomExtractors](../../groupdocs.search/indexsettings/customextractors) { get; } | Ottiene la raccolta di estrattori personalizzati. |
| [DocumentFilter](../../groupdocs.search/indexsettings/documentfilter) { get; set; } | Ottiene o imposta un filtro documento. Il [`DocumentFilter`](./documentfilter) funziona sulla logica di inclusione. Utilizza la classe [`DocumentFilter`](../../groupdocs.search.options/documentfilter) per creare istanze di filtri documento. Il valore predefinito è `null`, il che significa che tutti i documenti aggiunti vengono indicizzati. |
| [IndexType](../../groupdocs.search/indexsettings/indextype) { get; set; } | Ottiene o imposta il tipo di indice. Il valore predefinito è NormalIndex. |
| [InMemoryIndex](../../groupdocs.search/indexsettings/inmemoryindex) { get; } | Ottiene un valore che indica se l'indice è memorizzato in memoria o su disco. |
| [Logger](../../groupdocs.search/indexsettings/logger) { get; set; } | Ottiene o imposta un logger utilizzato per registrare eventi ed errori nell'indice. Nota che il logger non viene salvato e deve essere creato e assegnato ogni volta che l'indice viene creato o caricato. |
| [MaxIndexingReportCount](../../groupdocs.search/indexsettings/maxindexingreportcount) { get; set; } | Ottiene o imposta il numero massimo di report di indicizzazione. Il valore predefinito è `5`. |
| [MaxSearchReportCount](../../groupdocs.search/indexsettings/maxsearchreportcount) { get; set; } | Ottiene o imposta il numero massimo di report di ricerca. Il valore predefinito è `10`. |
| [SearchThreads](../../groupdocs.search/indexsettings/searchthreads) { get; set; } | Ottiene o imposta il numero di thread utilizzati per la ricerca. Il valore predefinito è Default, il che significa che la ricerca verrà eseguita usando un numero di thread pari al numero di core del processore. |
| [TextStorageSettings](../../groupdocs.search/indexsettings/textstoragesettings) { get; set; } | Ottiene o imposta le impostazioni di archiviazione del testo. Il valore predefinito è `null`, il che significa che i testi dei documenti non vengono memorizzati. |
| [UseCharacterReplacements](../../groupdocs.search/indexsettings/usecharacterreplacements) { get; set; } | Ottiene o imposta un valore che indica se utilizzare le sostituzioni di caratteri o meno. Il valore predefinito è `false`. |
| [UseStopWords](../../groupdocs.search/indexsettings/usestopwords) { get; set; } | Ottiene o imposta un valore che indica se utilizzare le parole stop o meno. Il valore predefinito è `true`. |

### Osservazioni

**Learn more**

* [Search index settings](https://docs.groupdocs.com/display/searchnet/Search+index+settings)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex; // Setting the index type

Index index = new Index(indexFolder, settings); // Creating an index
```

### Vedi anche

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
