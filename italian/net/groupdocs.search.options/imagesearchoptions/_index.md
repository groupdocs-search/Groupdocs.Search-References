---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce opzioni per l'operazione di ricerca inversa di immagini."
type: docs
weight: 960
url: /it/net/groupdocs.search.options/imagesearchoptions/
---
## ImageSearchOptions class

Fornisce opzioni per l'operazione di ricerca inversa di immagini.

```csharp
public class ImageSearchOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ImageSearchOptions](imagesearchoptions)() | Inizializza una nuova istanza della classe [`ImageSearchOptions`](../imagesearchoptions). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [HashDifferences](../../groupdocs.search.options/imagesearchoptions/hashdifferences) { get; set; } | Ottiene o imposta il numero massimo di bit non corrispondenti nell'hash dell'immagine. Il valore predefinito è `5`. |
| [MaxResultCount](../../groupdocs.search.options/imagesearchoptions/maxresultcount) { get; set; } | Ottiene o imposta il numero massimo di immagini trovate per una richiesta di ricerca inversa di immagini. Il valore predefinito è `1000`. |
| [SearchDocumentFilter](../../groupdocs.search.options/imagesearchoptions/searchdocumentfilter) { get; set; } | Ottiene o imposta il filtro del documento di ricerca. [`SearchDocumentFilter`](./searchdocumentfilter) funziona sulla logica di inclusione. Usa la classe [`SearchDocumentFilter`](../searchdocumentfilter) per creare istanze del filtro del documento di ricerca. Il valore predefinito è `null`, il che significa che tutti i documenti trovati saranno restituiti. |

### Vedi anche

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
