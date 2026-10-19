---
title: "IDocumentLoader"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Definisce l'interfaccia del caricatore di documenti utilizzata per caricare documenti lazy."
type: docs
weight: 180
url: /it/net/groupdocs.search.common/idocumentloader/
---
## IDocumentLoader interface

Definisce l'interfaccia del caricatore di documenti utilizzata per caricare documenti lazy.

```csharp
public interface IDocumentLoader
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CloseDocument](../../groupdocs.search.common/idocumentloader/closedocument)() | Chiude il documento caricato. Questo metodo è chiamato dall'indice quando ha terminato l'elaborazione del documento. |
| [LoadDocument](../../groupdocs.search.common/idocumentloader/loaddocument)() | Carica un documento. Questo metodo è chiamato dall'indice quando è pronto per elaborare il documento. |

### Vedi anche

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
