---
title: "UpdateOptions"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce opzioni per l'operazione di aggiornamento."
type: docs
weight: 1200
url: /it/net/groupdocs.search.options/updateoptions/
---
## UpdateOptions class

Fornisce opzioni per l'operazione di aggiornamento.

```csharp
public class UpdateOptions : BaseOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [UpdateOptions](updateoptions)() | Inizializza una nuova istanza della classe [`UpdateOptions`](../updateoptions). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Ottiene o imposta un valore che indica se rilevare automaticamente la codifica o meno. Il valore predefinito è `false`. |
| [Cancellation](../../groupdocs.search.options/updateoptions/cancellation) { get; set; } | Ottiene o imposta l'oggetto di annullamento dell'operazione. Il valore predefinito è `null`. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Ottiene o imposta la codifica usata per estrarre il testo dai documenti di testo. Il valore predefinito è `null`, il che significa che viene usata la codifica predefinita UTF-8. Se AutoDetectEncoding è `true` allora questo valore è usato come codifica predefinita. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Restituisce le opzioni di indicizzazione delle immagini per la ricerca inversa di immagini. |
| [IsAsync](../../groupdocs.search.options/updateoptions/isasync) { get; set; } | Ottiene o imposta il flag per l'esecuzione asincrona dell'operazione. Il valore predefinito è `false`. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Restituisce le opzioni per l'indicizzazione dei campi di metadati. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Restituisce le opzioni per l'elaborazione OCR e l'indicizzazione del testo riconosciuto. |
| [SeparateProcessOptions](../../groupdocs.search.options/updateoptions/separateprocessoptions) { get; } | Restituisce le opzioni per l'estrazione dei dati in un processo separato. |
| [Threads](../../groupdocs.search.options/updateoptions/threads) { get; set; } | Ottiene o imposta il numero di thread utilizzati per l'indicizzazione. Il valore predefinito è `1`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Ottiene o imposta un valore che indica se il processo deve utilizzare SeBackupPrivilege e FILE_FLAG_BACKUP_SEMANTICS per accedere a file e directory. Il valore predefinito è `false`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Ottiene o imposta un valore che indica se utilizzare la modalità grezza per l'estrazione del testo, se possibile. Il valore predefinito è `false`. La modalità grezza può aumentare notevolmente la velocità di indicizzazione, ma la modalità normale migliora la formattazione del testo estratto. |

### Osservazioni

**Learn more**

* [Update index](https://docs.groupdocs.com/display/searchnet/Update+index)
* [Delete indexed paths](https://docs.groupdocs.com/display/searchnet/Delete+indexed+paths)

### Vedi anche

* class [BaseOptions](../baseoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
