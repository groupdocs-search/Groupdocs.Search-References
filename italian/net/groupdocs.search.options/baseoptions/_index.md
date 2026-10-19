---
title: "BaseOptions"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce opzioni di base per le operazioni di indicizzazione."
type: docs
weight: 760
url: /it/net/groupdocs.search.options/baseoptions/
---
## BaseOptions class

Fornisce opzioni di base per le operazioni di indicizzazione.

```csharp
public abstract class BaseOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [BaseOptions](baseoptions)() | Inizializza una nuova istanza della classe [`BaseOptions`](../baseoptions). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Ottiene o imposta un valore che indica se rilevare automaticamente la codifica o meno. Il valore predefinito è `false`. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Ottiene o imposta la codifica usata per estrarre il testo dai documenti di testo. Il valore predefinito è `null`, il che significa che viene usata la codifica predefinita UTF-8. Se AutoDetectEncoding è `true` allora questo valore è usato come codifica predefinita. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Restituisce le opzioni di indicizzazione delle immagini per la ricerca inversa di immagini. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Restituisce le opzioni per l'indicizzazione dei campi di metadati. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Restituisce le opzioni per l'elaborazione OCR e l'indicizzazione del testo riconosciuto. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Ottiene o imposta un valore che indica se il processo deve utilizzare SeBackupPrivilege e FILE_FLAG_BACKUP_SEMANTICS per accedere a file e directory. Il valore predefinito è `false`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Ottiene o imposta un valore che indica se utilizzare la modalità grezza per l'estrazione del testo, se possibile. Il valore predefinito è `false`. La modalità grezza può aumentare notevolmente la velocità di indicizzazione, ma la modalità normale migliora la formattazione del testo estratto. |

### Vedi anche

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
