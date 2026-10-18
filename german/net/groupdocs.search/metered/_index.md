---
title: "Abgerechnet"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Methoden bereit, die es ermöglichen, das Produkt mit einer Metered-Lizenz zu aktivieren und die Menge der verarbeiteten MB abzurufen. Erfahren Sie mehr über Metered-Lizenzen hierhttps//purchase.groupdocs.com/faqs/licensing/metered."
type: docs
weight: 750
url: /de/net/groupdocs.search/metered/
---
## Metered class

Bietet Methoden, die es ermöglichen, das Produkt mit einer nutzungsbasierten Lizenz zu aktivieren und die verarbeiteten MB-Mengen abzurufen. Weitere Informationen zu nutzungsbasierten Lizenzen finden Sie [hier](https://purchase.groupdocs.com/faqs/licensing/metered).

```csharp
public class Metered
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Metered](metered)() | Initialisiert eine neue Instanz der [`Metered`](../metered)-Klasse. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetMeteredKey](../../groupdocs.search/metered/setmeteredkey)(string, string) | Setzt den öffentlichen und privaten Metered-Schlüssel. |
| static [GetConsumptionCredit](../../groupdocs.search/metered/getconsumptioncredit)() | Liefert das Verbrauchsguthaben. |
| static [GetConsumptionQuantity](../../groupdocs.search/metered/getconsumptionquantity)() | Liefert die Verbrauchsmenge. |

### Hinweise

**Learn more**

* [Evaluation Limitations and Licensing](https://docs.groupdocs.com/display/searchnet/Evaluation+Limitations+and+Licensing)

### Beispiele

Das Beispiel zeigt, wie man öffentliche und private Metered-Schlüssel setzt.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");
```

### Siehe auch

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
