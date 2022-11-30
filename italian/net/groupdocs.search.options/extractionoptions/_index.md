---
title: ExtractionOptions
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Fornisce opzioni per lestrazione di dati dai documenti.
type: docs
weight: 790
url: /it/net/groupdocs.search.options/extractionoptions/
---
## ExtractionOptions class

Fornisce opzioni per l'estrazione di dati dai documenti.

```csharp
public class ExtractionOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ExtractionOptions](extractionoptions)() | Inizializza una nuova istanza di[`ExtractionOptions`](../extractionoptions) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CustomExtractor](../../groupdocs.search.options/extractionoptions/customextractor) { get; set; } | Ottiene o imposta l'estrattore di testo personalizzato. Il valore predefinito è`nullo` . |
| [Encoding](../../groupdocs.search.options/extractionoptions/encoding) { get; set; } | Ottiene o imposta la codifica utilizzata per l'estrazione dai documenti di testo. |
| [ImageIndexingOptions](../../groupdocs.search.options/extractionoptions/imageindexingoptions) { get; } | Ottiene le opzioni di indicizzazione delle immagini per la ricerca inversa delle immagini. |
| [MetadataIndexingOptions](../../groupdocs.search.options/extractionoptions/metadataindexingoptions) { get; } | Ottiene le opzioni per l'indicizzazione dei campi dei metadati. |
| [OcrIndexingOptions](../../groupdocs.search.options/extractionoptions/ocrindexingoptions) { get; } | Ottiene le opzioni per l'elaborazione OCR e l'indicizzazione del testo riconosciuto. |
| [UseRawTextExtraction](../../groupdocs.search.options/extractionoptions/userawtextextraction) { get; set; } | Ottiene o imposta un valore che indica se la modalità raw viene utilizzata per l'estrazione del testo, se possibile. Il valore predefinito è`VERO` . La modalità raw può aumentare significativamente la velocità di indicizzazione, ma la modalità normale migliora la formattazione del testo estratto. |

### Guarda anche

* spazio dei nomi [GroupDocs.Search.Options](../../groupdocs.search.options)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->