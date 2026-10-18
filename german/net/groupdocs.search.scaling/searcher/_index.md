---
title: "Sucher"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Dienst dar, der Suchanfragen an die Shards des Suchnetzwerks verwaltet."
type: docs
weight: 1570
url: /de/net/groupdocs.search.scaling/searcher/
---
## Searcher class

Stellt einen Dienst dar, der Suchanfragen an die Shards des Suchnetzwerks verwaltet.

```csharp
public sealed class Searcher
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetDocumentText](../../groupdocs.search.scaling/searcher/getdocumenttext)(NetworkDocumentInfo, OutputAdapter) | Erzeugt den Text eines indexierten Dokuments und leitet ihn über einen Ausgabeadapter weiter. |
| [GetIndexedDocumentItems](../../groupdocs.search.scaling/searcher/getindexeddocumentitems)(NetworkDocumentInfo) | Gibt ein Array verschachtelter Elemente des angegebenen Dokuments zurück (für Container-Dokumente wie ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search.scaling/searcher/getindexeddocuments)(int) | Gibt ein Array aller indizierten Dokumente zurück. |
| [Highlight](../../groupdocs.search.scaling/searcher/highlight)(NetworkFoundDocument, Highlighter, HighlightOptions) | Erzeugt HTML-formatierten Text mit hervorgehobenen gefundenen Begriffen. |
| [SearchFirst](../../groupdocs.search.scaling/searcher/searchfirst#searchfirst)(SearchImage, ImageSearchOptions) | Startet eine umgekehrte Bildsuche im verteilten Suchindex. |
| [SearchFirst](../../groupdocs.search.scaling/searcher/searchfirst#searchfirst_1)(SearchQuery, SearchOptions) | Startet eine Suche mit einer Abfrage in Objektform im verteilten Suchindex. |
| [SearchFirst](../../groupdocs.search.scaling/searcher/searchfirst#searchfirst_2)(string, SearchOptions) | Startet eine Suche mit einer Abfrage in Textform im verteilten Suchindex. |
| [SearchNext](../../groupdocs.search.scaling/searcher/searchnext#searchnext)(NetworkImageSearchToken) | Fährt mit einer umgekehrten Bildsuche im verteilten Suchindex fort. |
| [SearchNext](../../groupdocs.search.scaling/searcher/searchnext#searchnext_1)(NetworkSearchToken) | Fährt mit einer Suche im verteilten Suchindex fort. |

### Siehe auch

* namespace [GroupDocs.Search.Scaling](../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
