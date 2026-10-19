---
title: "Metered"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce metodi che consentono di attivare il prodotto con licenza Metered e recuperare la quantità di MB elaborati. Scopri di più sulle licenze Metered quihttps//purchase.groupdocs.com/faqs/licensing/metered."
type: docs
weight: 750
url: /it/net/groupdocs.search/metered/
---
## Metered class

Fornisce metodi che consentono di attivare il prodotto con licenza a consumo e recuperare la quantità di MB elaborati. Scopri di più sulle licenze a consumo [qui](https://purchase.groupdocs.com/faqs/licensing/metered).

```csharp
public class Metered
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Metered](metered)() | Inizializza una nuova istanza della classe [`Metered`](../metered). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetMeteredKey](../../groupdocs.search/metered/setmeteredkey)(string, string) | Imposta la chiave pubblica e privata per la licenza Metered. |
| static [GetConsumptionCredit](../../groupdocs.search/metered/getconsumptioncredit)() | Ottiene il credito di consumo. |
| static [GetConsumptionQuantity](../../groupdocs.search/metered/getconsumptionquantity)() | Ottiene la quantità di consumo. |

### Osservazioni

**Learn more**

* [Evaluation Limitations and Licensing](https://docs.groupdocs.com/display/searchnet/Evaluation+Limitations+and+Licensing)

### Esempi

L'esempio dimostra come impostare le chiavi pubbliche e private a consumo.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");
```

### Vedi anche

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
