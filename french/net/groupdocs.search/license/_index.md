---
title: "License"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des méthodes pour appliquer la licence."
type: docs
weight: 740
url: /fr/net/groupdocs.search/license/
---
## License class

Fournit des méthodes pour appliquer la licence.

```csharp
public sealed class License
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [License](license)() | Initialise une nouvelle instance de la classe [`License`](../license). |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense)(Stream) | Licence le composant. |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense_1)(string) | Licence le composant. |

### Remarques

**Learn more**

* [Evaluation Limitations and Licensing](https://docs.groupdocs.com/display/searchnet/Evaluation+Limitations+and+Licensing)

### Exemples

L'exemple montre comment configurer la licence.

```csharp
License license = new License();
license.SetLicense("C:\\GroupDocs.Search.lic");
```

### Voir aussi

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
