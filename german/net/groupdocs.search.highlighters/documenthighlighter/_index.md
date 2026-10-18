---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Suchergebnis‑Highlighter dar, der Suchergebnisse im gesamten Dokumenttext hervorhebt."
type: docs
weight: 670
url: /de/net/groupdocs.search.highlighters/documenthighlighter/
---
## DocumentHighlighter class

Stellt einen Suchergebnis‑Highlighter dar, der Suchergebnisse im gesamten Dokumenttext hervorhebt.

```csharp
public class DocumentHighlighter : Highlighter
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [DocumentHighlighter](documenthighlighter)(OutputAdapter) | Initialisiert eine neue Instanz der Klasse [`DocumentHighlighter`](../documenthighlighter). |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [OutputAdapter](../../groupdocs.search.highlighters/documenthighlighter/outputadapter) { get; } | Liefert den im Konstruktor übergebenen Ausgabeadapter. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Liefert das Ausgabeformat. |

### Hinweise

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);

// Suche nach der Phrase 'Theory of Relativity'
SearchResult result = index.Search("\"Theory of Relativity\"");

// Markieren gefundener Wörter im Text eines Dokuments
FoundDocument document = result.GetFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.Highlight(document, highlighter);
```

### Siehe auch

* class [Highlighter](../highlighter)
* namespace [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
