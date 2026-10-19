---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Contiene una raccolta di estrattori personalizzati. Se la raccolta contiene un estrattore per qualche estensione di file coperta dagli estrattori integrati, allora questo estrattore verrà utilizzato al posto di quello integrato."
type: docs
weight: 40
url: /it/net/groupdocs.search.common/customextractorcollection/
---
## CustomExtractorCollection class

Contiene una raccolta di estrattori personalizzati. Se la raccolta contiene un estrattore per qualche estensione di file coperta dagli estrattori integrati, allora questo estrattore verrà utilizzato al posto di quello integrato.

```csharp
public class CustomExtractorCollection : ICollection<IFieldExtractor>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.search.common/customextractorcollection/count) { get; } | Restituisce il numero di estrattori contenuti nella raccolta. |
| [IsReadOnly](../../groupdocs.search.common/customextractorcollection/isreadonly) { get; } | Restituisce un valore che indica se la raccolta è di sola lettura. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../groupdocs.search.common/customextractorcollection/add)(IFieldExtractor) | Aggiunge un estrattore alla raccolta. |
| [Clear](../../groupdocs.search.common/customextractorcollection/clear)() | Rimuove tutti gli estrattori dalla raccolta. |
| [Contains](../../groupdocs.search.common/customextractorcollection/contains)(IFieldExtractor) | Determina se la raccolta contiene un estrattore specifico. |
| [CopyTo](../../groupdocs.search.common/customextractorcollection/copyto)(IFieldExtractor[], int) | Copia gli elementi della raccolta in un array, iniziando da un indice specifico dell'array. |
| [GetEnumerator](../../groupdocs.search.common/customextractorcollection/getenumerator)() | Restituisce un enumeratore per questa raccolta. |
| [Remove](../../groupdocs.search.common/customextractorcollection/remove)(IFieldExtractor) | Rimuove un estrattore dalla raccolta. |

### Osservazioni

**Learn more**

* [Custom text extractors](https://docs.groupdocs.com/display/searchnet/Custom+text+extractors)

### Vedi anche

* interface [IFieldExtractor](../ifieldextractor)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
