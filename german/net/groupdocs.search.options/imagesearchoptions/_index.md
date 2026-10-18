---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Optionen für die umgekehrte Bildsuche-Operation bereit."
type: docs
weight: 960
url: /de/net/groupdocs.search.options/imagesearchoptions/
---
## ImageSearchOptions class

Stellt Optionen für die umgekehrte Bildsuche-Operation bereit.

```csharp
public class ImageSearchOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ImageSearchOptions](imagesearchoptions)() | Initialisiert eine neue Instanz der Klasse [`ImageSearchOptions`](../imagesearchoptions). |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [HashDifferences](../../groupdocs.search.options/imagesearchoptions/hashdifferences) { get; set; } | Liest oder legt die maximale Anzahl nicht übereinstimmender Bits im Bild-Hash fest. Der Standardwert ist `5`. |
| [MaxResultCount](../../groupdocs.search.options/imagesearchoptions/maxresultcount) { get; set; } | Liest oder legt die maximale Anzahl gefundener Bilder für eine Bild-Rückwärtssuche fest. Der Standardwert ist `1000`. |
| [SearchDocumentFilter](../../groupdocs.search.options/imagesearchoptions/searchdocumentfilter) { get; set; } | Liest oder legt den Suchdokumentfilter fest. [`SearchDocumentFilter`](./searchdocumentfilter) arbeitet nach der Einschlusslogik. Verwenden Sie die Klasse [`SearchDocumentFilter`](../searchdocumentfilter) zur Erstellung von Suchdokumentfilterinstanzen. Der Standardwert ist `null`, was bedeutet, dass alle gefundenen Dokumente zurückgegeben werden. |

### Siehe auch

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
