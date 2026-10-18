---
title: "HighlightOptions"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Optionen zum Hervorheben gefundener Begriffe bereit."
type: docs
weight: 910
url: /de/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Stellt Optionen zum Hervorheben gefundener Begriffe bereit.

```csharp
public class HighlightOptions : TextOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Initialisiert eine neue Instanz der Klasse [`HighlightOptions`](../highlightoptions). |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Liest oder setzt die zusätzlichen Dokumentfelder, die für die Indizierung verwendet wurden. Der Standardwert ist `null`. Hinweis: Dieser Wert wird nur verwendet, wenn der Dokumenttext nicht im Index gespeichert wurde. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Kodierung automatisch erkannt werden soll oder nicht. Der Standardwert ist `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Liest oder setzt das Abbruchobjekt. Der Standardwert ist `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Liest oder setzt den benutzerdefinierten Textextraktor, der für die Indizierung verwendet wurde. Der Standardwert ist `null`. Hinweis: Dieser Wert wird nur verwendet, wenn der Dokumenttext nicht im Index gespeichert wurde. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Liest oder setzt die Kodierung, die zum Extrahieren von Text aus Textdokumenten verwendet wird. Der Standardwert ist `null`, was bedeutet, dass die Standardkodierung UTF-8 verwendet wird. Ist AutoDetectEncoding `true`, wird dieser Wert als Standardkodierung verwendet. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Liest oder setzt einen Wert, der angibt, ob das Head-Tag im ausgegebenen HTML erzeugt wird. Der Standardwert ist `true`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Liest oder setzt eine Farbe, die zum Hervorheben von Vorkommen verwendet wird. Der Standardwert ist #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Liest die Bildindizierungsoptionen für die umgekehrte Bildsuche. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Liest die Optionen für die Indizierung von Metadatenfeldern. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Liest die Optionen für die OCR-Verarbeitung und das Indizieren von erkanntem Text. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Liest oder setzt das End-Tag für die Hervorhebung des gefundenen Wortes. Dieses Tag wird nur verwendet, wenn im Nur-Text hervorgehoben wird. Der Standardwert ist ein leerer String. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Liest oder setzt das Start-Tag für die Hervorhebung des gefundenen Wortes. Dieses Tag wird nur verwendet, wenn im Nur-Text hervorgehoben wird. Der Standardwert ist ein leerer String. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Liest oder setzt die maximale Anzahl von Wörtern in einem Textfragment nach dem hervorgehobenen Wort. Der Wert muss im Bereich von 0 bis 10000 liegen. Der Standardwert ist `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Liest oder setzt die maximale Anzahl von Wörtern in einem Textfragment vor dem hervorgehobenen Wort. Der Wert muss im Bereich von 0 bis 10000 liegen. Der Standardwert ist `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Liest oder setzt die maximale Anzahl von Wörtern in einem Textfragment. Der Wert muss im Bereich von 0 bis 10000 liegen. Der Standardwert ist `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Prozess das SeBackupPrivilege und FILE_FLAG_BACKUP_SEMANTICS zum Zugriff auf Dateien und Verzeichnisse verwenden soll. Der Standardwert ist `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Liest oder setzt einen Wert, der angibt, ob Inline‑Stile zum Hervorheben von Vorkommen verwendet werden. Der Standardwert ist `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Rohmodus für die Textextraktion, falls möglich, verwendet wird. Der Standardwert ist `false`. Der Rohmodus kann die Indizierungsgeschwindigkeit erheblich steigern, aber der Normalmodus verbessert die Formatierung des extrahierten Textes. |

### Hinweise

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Siehe auch

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
