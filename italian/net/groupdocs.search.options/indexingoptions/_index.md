---
title: "IndexingOptions"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce opzioni per l'operazione di indicizzazione."
type: docs
weight: 980
url: /it/net/groupdocs.search.options/indexingoptions/
---
## IndexingOptions class

Fornisce opzioni per l'operazione di indicizzazione.

```csharp
public class IndexingOptions : BaseOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [IndexingOptions](indexingoptions)() | Inizializza una nuova istanza della classe [`IndexingOptions`](../indexingoptions). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Ottiene o imposta un valore che indica se rilevare automaticamente la codifica o meno. Il valore predefinito è `false`. |
| [Cancellation](../../groupdocs.search.options/indexingoptions/cancellation) { get; set; } | Ottiene o imposta l'oggetto di annullamento dell'operazione. Il valore predefinito è `null`. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Ottiene o imposta la codifica usata per estrarre il testo dai documenti di testo. Il valore predefinito è `null`, il che significa che viene usata la codifica predefinita UTF-8. Se AutoDetectEncoding è `true` allora questo valore è usato come codifica predefinita. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Restituisce le opzioni di indicizzazione delle immagini per la ricerca inversa di immagini. |
| [IsAsync](../../groupdocs.search.options/indexingoptions/isasync) { get; set; } | Ottiene o imposta il flag per l'esecuzione asincrona dell'operazione. Il valore predefinito è `false`. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Restituisce le opzioni per l'indicizzazione dei campi di metadati. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Restituisce le opzioni per l'elaborazione OCR e l'indicizzazione del testo riconosciuto. |
| [SeparateProcessOptions](../../groupdocs.search.options/indexingoptions/separateprocessoptions) { get; } | Restituisce le opzioni per l'estrazione dei dati in un processo separato. |
| [Threads](../../groupdocs.search.options/indexingoptions/threads) { get; set; } | Ottiene o imposta il numero di thread utilizzati per l'indicizzazione. Il parametro deve essere compreso nell'intervallo da `1` a `4`. Il valore predefinito è `1`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Ottiene o imposta un valore che indica se il processo deve utilizzare SeBackupPrivilege e FILE_FLAG_BACKUP_SEMANTICS per accedere a file e directory. Il valore predefinito è `false`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Ottiene o imposta un valore che indica se utilizzare la modalità grezza per l'estrazione del testo, se possibile. Il valore predefinito è `false`. La modalità grezza può aumentare notevolmente la velocità di indicizzazione, ma la modalità normale migliora la formattazione del testo estratto. |

### Osservazioni

**Learn more**

* [Indexing options](https://docs.groupdocs.com/display/searchnet/Indexing+options)

### Vedi anche

* class [BaseOptions](../baseoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
