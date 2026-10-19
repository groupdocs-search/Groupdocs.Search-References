---
title: "Estrattore"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta uno strumento per l'estrazione preliminare dei dati dai documenti, al fine di separare la fase di indicizzazione rapida successiva."
type: docs
weight: 660
url: /it/net/groupdocs.search/extractor/
---
## Extractor class

Rappresenta uno strumento per l'estrazione preliminare dei dati dai documenti, al fine di separare la fase di indicizzazione rapida successiva.

```csharp
public class Extractor
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Extractor](extractor)() | Inizializza una nuova istanza della classe [`Extractor`](../extractor). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Settings](../../groupdocs.search/extractor/settings) { get; } | Ottiene le impostazioni dell'estrattore. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Extract](../../groupdocs.search/extractor/extract)(Document, ExtractionOptions) | Estrae dati da un documento. |

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [ErrorOccurred](../../groupdocs.search/extractor/erroroccurred) | Si verifica quando si verifica un errore durante un'operazione dell'estrattore. |
| event [ImagePreparing](../../groupdocs.search/extractor/imagepreparing) | Si verifica quando un'immagine sta per essere preparata per l'indicizzazione. |
| event [PasswordRequired](../../groupdocs.search/extractor/passwordrequired) | Si verifica quando un documento richiede una password per l'apertura. |

### Vedi anche

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
