---
title: "License"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce metodi per applicare la licenza."
type: docs
weight: 740
url: /it/net/groupdocs.search/license/
---
## License class

Fornisce metodi per applicare la licenza.

```csharp
public sealed class License
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [License](license)() | Inizializza una nuova istanza della classe [`License`](../license). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense)(Stream) | Concede la licenza al componente. |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense_1)(string) | Concede la licenza al componente. |

### Osservazioni

**Learn more**

* [Evaluation Limitations and Licensing](https://docs.groupdocs.com/display/searchnet/Evaluation+Limitations+and+Licensing)

### Esempi

L'esempio dimostra come configurare la licenza.

```csharp
License license = new License();
license.SetLicense("C:\\GroupDocs.Search.lic");
```

### Vedi anche

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
