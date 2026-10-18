---
title: "Suchoptionen"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Optionen für die Suchoperation bereit."
type: docs
weight: 1100
url: /de/net/groupdocs.search.options/searchoptions/
---
## SearchOptions class

Stellt Optionen für die Suchoperation bereit.

```csharp
public class SearchOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SearchOptions](searchoptions)() | Initialisiert eine neue Instanz der [`SearchOptions`](../searchoptions)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Cancellation](../../groupdocs.search.options/searchoptions/cancellation) { get; set; } | Liest oder setzt das Abbruchobjekt der Operation. Der Standardwert ist `null`. |
| [DateFormats](../../groupdocs.search.options/searchoptions/dateformats) { get; } | Liefert die Sammlung von Datumsformaten für die Datumsspanne‑Suche. Die Standard‑Datumsformate sind 'dd.MM.yyyy', 'MM/dd/yyyy' und 'yyyy-MM-dd'. |
| [FuzzySearch](../../groupdocs.search.options/searchoptions/fuzzysearch) { get; } | Liefert die Optionen für unscharfe Suche. |
| [IsChunkSearch](../../groupdocs.search.options/searchoptions/ischunksearch) { get; set; } | Liefert oder setzt das Flag für die Suche in Abschnitten. Der Standardwert ist `false`. |
| [KeyboardLayoutCorrector](../../groupdocs.search.options/searchoptions/keyboardlayoutcorrector) { get; } | Liefert die Optionen für die Korrektur der Tastaturbelegung. |
| [MaxOccurrenceCountPerTerm](../../groupdocs.search.options/searchoptions/maxoccurrencecountperterm) { get; set; } | Liefert oder setzt die maximale Anzahl von Vorkommen jedes Begriffs in einer Suchanfrage. Der Standardwert ist `2000000000`. |
| [MaxTotalOccurrenceCount](../../groupdocs.search.options/searchoptions/maxtotaloccurrencecount) { get; set; } | Liefert oder setzt die maximale Gesamtzahl von Vorkommen aller Begriffe in einer Suchanfrage. Der Standardwert ist `2000000000`. |
| [RetrieveAttributes](../../groupdocs.search.options/searchoptions/retrieveattributes) { get; set; } | Liefert oder setzt das Flag zum Abrufen von Attributen, die mit gefundenen Dokumenten verknüpft sind. Der Standardwert ist `false`. |
| [SearchDocumentFilter](../../groupdocs.search.options/searchoptions/searchdocumentfilter) { get; set; } | Liest oder legt den Suchdokumentfilter fest. [`SearchDocumentFilter`](./searchdocumentfilter) arbeitet nach der Einschlusslogik. Verwenden Sie die Klasse [`SearchDocumentFilter`](../searchdocumentfilter) zur Erstellung von Suchdokumentfilterinstanzen. Der Standardwert ist `null`, was bedeutet, dass alle gefundenen Dokumente zurückgegeben werden. |
| [SpellingCorrector](../../groupdocs.search.options/searchoptions/spellingcorrector) { get; } | Liefert die Optionen für die Rechtschreibkorrektur. |
| [UseCaseSensitiveSearch](../../groupdocs.search.options/searchoptions/usecasesensitivesearch) { get; set; } | Liefert oder setzt das Flag für die Groß‑/Kleinschreibung bei der Suche. Der Standardwert ist `false`. |
| [UseHomophoneSearch](../../groupdocs.search.options/searchoptions/usehomophonesearch) { get; set; } | Liefert oder setzt das Flag zur Verwendung von Homophonen in der Suche. Der Standardwert ist `false`. |
| [UseSynonymSearch](../../groupdocs.search.options/searchoptions/usesynonymsearch) { get; set; } | Liefert oder setzt das Flag zur Verwendung von Synonymen in der Suche. Der Standardwert ist `false`. |
| [UseWordFormsSearch](../../groupdocs.search.options/searchoptions/usewordformssearch) { get; set; } | Liefert oder setzt das Flag zur Verwendung verschiedener Wortformen in der Suche. Der Standardwert ist `false`. |

### Hinweise

**Learn more**

* [Search options](https://docs.groupdocs.com/display/searchnet/Search+options)

### Siehe auch

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
