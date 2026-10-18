---
title: "License"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Bietet Methoden zum Anwenden einer Lizenz."
type: docs
weight: 740
url: /de/net/groupdocs.search/license/
---
## License class

Bietet Methoden zum Anwenden einer Lizenz.

```csharp
public sealed class License
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [License](license)() | Initialisiert eine neue Instanz der [`License`](../license)-Klasse. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense)(Stream) | Lizenziert die Komponente. |
| [SetLicense](../../groupdocs.search/license/setlicense#setlicense_1)(string) | Lizenziert die Komponente. |

### Hinweise

**Learn more**

* [Evaluation Limitations and Licensing](https://docs.groupdocs.com/display/searchnet/Evaluation+Limitations+and+Licensing)

### Beispiele

Das Beispiel zeigt, wie man die Lizenz einrichtet.

```csharp
License license = new License();
license.SetLicense("C:\\GroupDocs.Search.lic");
```

### Siehe auch

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
