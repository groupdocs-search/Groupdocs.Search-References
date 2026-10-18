---
title: "Metered"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des méthodes qui permettent d'activer le produit avec une licence Metered et de récupérer la quantité de Mo traités. En savoir plus sur les licences Metered icihttps//purchase.groupdocs.com/faqs/licensing/metered."
type: docs
weight: 750
url: /fr/net/groupdocs.search/metered/
---
## Metered class

Fournit des méthodes qui permettent d'activer le produit avec une licence à consommation et de récupérer la quantité de Mo traités. En savoir plus sur les licences à consommation [ici](https://purchase.groupdocs.com/faqs/licensing/metered).

```csharp
public class Metered
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Metered](metered)() | Initialise une nouvelle instance de la classe [`Metered`](../metered). |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetMeteredKey](../../groupdocs.search/metered/setmeteredkey)(string, string) | Définit la clé publique et privée Metered. |
| static [GetConsumptionCredit](../../groupdocs.search/metered/getconsumptioncredit)() | Obtient le crédit de consommation. |
| static [GetConsumptionQuantity](../../groupdocs.search/metered/getconsumptionquantity)() | Obtient la quantité de consommation. |

### Remarques

**Learn more**

* [Evaluation Limitations and Licensing](https://docs.groupdocs.com/display/searchnet/Evaluation+Limitations+and+Licensing)

### Exemples

L'exemple montre comment définir les clés publiques et privées mesurées.

```csharp
Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");
```

### Voir aussi

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
