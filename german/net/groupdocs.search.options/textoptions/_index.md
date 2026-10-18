---
title: "TextOptions"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Optionen zum Abrufen von Dokumenttext aus einem Index bereit."
type: docs
weight: 1180
url: /de/net/groupdocs.search.options/textoptions/
---
## TextOptions class

Stellt Optionen zum Abrufen von Dokumenttext aus einem Index bereit.

```csharp
public class TextOptions : BaseOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TextOptions](textoptions)() | Initialisiert eine neue Instanz der [`TextOptions`](../textoptions)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Liest oder setzt die zusätzlichen Dokumentfelder, die für die Indizierung verwendet wurden. Der Standardwert ist `null`. Hinweis: Dieser Wert wird nur verwendet, wenn der Dokumenttext nicht im Index gespeichert wurde. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Kodierung automatisch erkannt werden soll oder nicht. Der Standardwert ist `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Liest oder setzt das Abbruchobjekt. Der Standardwert ist `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Liest oder setzt den benutzerdefinierten Textextraktor, der für die Indizierung verwendet wurde. Der Standardwert ist `null`. Hinweis: Dieser Wert wird nur verwendet, wenn der Dokumenttext nicht im Index gespeichert wurde. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Liest oder setzt die Kodierung, die zum Extrahieren von Text aus Textdokumenten verwendet wird. Der Standardwert ist `null`, was bedeutet, dass die Standardkodierung UTF-8 verwendet wird. Ist AutoDetectEncoding `true`, wird dieser Wert als Standardkodierung verwendet. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Liest oder setzt einen Wert, der angibt, ob das Head-Tag im ausgegebenen HTML erzeugt wird. Der Standardwert ist `true`. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Liest die Bildindizierungsoptionen für die umgekehrte Bildsuche. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Liest die Optionen für die Indizierung von Metadatenfeldern. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Liest die Optionen für die OCR-Verarbeitung und das Indizieren von erkanntem Text. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Prozess das SeBackupPrivilege und FILE_FLAG_BACKUP_SEMANTICS zum Zugriff auf Dateien und Verzeichnisse verwenden soll. Der Standardwert ist `false`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Rohmodus für die Textextraktion, falls möglich, verwendet wird. Der Standardwert ist `false`. Der Rohmodus kann die Indizierungsgeschwindigkeit erheblich steigern, aber der Normalmodus verbessert die Formatierung des extrahierten Textes. |

### Hinweise

**Learn more**

* [Getting indexed documents](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)
* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Siehe auch

* class [BaseOptions](../baseoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
