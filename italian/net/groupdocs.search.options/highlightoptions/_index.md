---
title: "HighlightOptions"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce opzioni per evidenziare i termini trovati."
type: docs
weight: 910
url: /it/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Fornisce opzioni per evidenziare i termini trovati.

```csharp
public class HighlightOptions : TextOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Inizializza una nuova istanza della classe [`HighlightOptions`](../highlightoptions). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Ottiene o imposta i campi aggiuntivi del documento che sono stati usati per l'indicizzazione. Il valore predefinito è `null`. Nota che questo valore è usato solo se il testo del documento non è stato salvato nell'indice. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Ottiene o imposta un valore che indica se rilevare automaticamente la codifica o meno. Il valore predefinito è `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Ottiene o imposta l'oggetto di cancellazione. Il valore predefinito è `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Ottiene o imposta l'estrattore di testo personalizzato che è stato usato per l'indicizzazione. Il valore predefinito è `null`. Nota che questo valore è usato solo se il testo del documento non è stato salvato nell'indice. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Ottiene o imposta la codifica usata per estrarre il testo dai documenti di testo. Il valore predefinito è `null`, il che significa che viene usata la codifica predefinita UTF-8. Se AutoDetectEncoding è `true` allora questo valore è usato come codifica predefinita. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Ottiene o imposta un valore che indica se il tag Head è generato nell'HTML di output. Il valore predefinito è `true`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Ottiene o imposta un colore usato per evidenziare le occorrenze. Il valore predefinito è #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Restituisce le opzioni di indicizzazione delle immagini per la ricerca inversa di immagini. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Restituisce le opzioni per l'indicizzazione dei campi di metadati. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Restituisce le opzioni per l'elaborazione OCR e l'indicizzazione del testo riconosciuto. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Ottiene o imposta il tag di chiusura per l'evidenziazione della parola trovata. Questo tag è usato solo durante l'evidenziazione in testo semplice. Il valore predefinito è una stringa vuota. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Ottiene o imposta il tag di apertura per l'evidenziazione della parola trovata. Questo tag è usato solo durante l'evidenziazione in testo semplice. Il valore predefinito è una stringa vuota. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Ottiene o imposta il numero massimo di parole in un frammento di testo dopo la parola evidenziata. Il valore deve essere compreso tra 0 e 10000. Il valore predefinito è `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Ottiene o imposta il numero massimo di parole in un frammento di testo prima della parola evidenziata. Il valore deve essere compreso tra 0 e 10000. Il valore predefinito è `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Ottiene o imposta il numero massimo di parole in un frammento di testo. Il valore deve essere compreso tra 0 e 10000. Il valore predefinito è `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Ottiene o imposta un valore che indica se il processo deve utilizzare SeBackupPrivilege e FILE_FLAG_BACKUP_SEMANTICS per accedere a file e directory. Il valore predefinito è `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Ottiene o imposta un valore che indica se vengono usati stili inline per evidenziare le occorrenze. Il valore predefinito è `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Ottiene o imposta un valore che indica se utilizzare la modalità grezza per l'estrazione del testo, se possibile. Il valore predefinito è `false`. La modalità grezza può aumentare notevolmente la velocità di indicizzazione, ma la modalità normale migliora la formattazione del testo estratto. |

### Osservazioni

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Vedi anche

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
