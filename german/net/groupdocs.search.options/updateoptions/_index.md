---
title: "UpdateOptions"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Bietet Optionen für den Aktualisierungsvorgang."
type: docs
weight: 1200
url: /de/net/groupdocs.search.options/updateoptions/
---
## UpdateOptions class

Bietet Optionen für den Aktualisierungsvorgang.

```csharp
public class UpdateOptions : BaseOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [UpdateOptions](updateoptions)() | Initialisiert eine neue Instanz der Klasse [`UpdateOptions`](../updateoptions). |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Kodierung automatisch erkannt werden soll oder nicht. Der Standardwert ist `false`. |
| [Cancellation](../../groupdocs.search.options/updateoptions/cancellation) { get; set; } | Liest oder setzt das Abbruchobjekt der Operation. Der Standardwert ist `null`. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Liest oder setzt die Kodierung, die zum Extrahieren von Text aus Textdokumenten verwendet wird. Der Standardwert ist `null`, was bedeutet, dass die Standardkodierung UTF-8 verwendet wird. Ist AutoDetectEncoding `true`, wird dieser Wert als Standardkodierung verwendet. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Liest die Bildindizierungsoptionen für die umgekehrte Bildsuche. |
| [IsAsync](../../groupdocs.search.options/updateoptions/isasync) { get; set; } | Liest oder setzt das Flag für die asynchrone Ausführung der Operation. Der Standardwert ist `false`. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Liest die Optionen für die Indizierung von Metadatenfeldern. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Liest die Optionen für die OCR-Verarbeitung und das Indizieren von erkanntem Text. |
| [SeparateProcessOptions](../../groupdocs.search.options/updateoptions/separateprocessoptions) { get; } | Liest die Optionen zum Extrahieren von Daten in einem separaten Prozess. |
| [Threads](../../groupdocs.search.options/updateoptions/threads) { get; set; } | Liest oder setzt die Anzahl der für die Indizierung verwendeten Threads. Der Standardwert ist `1`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Prozess das SeBackupPrivilege und FILE_FLAG_BACKUP_SEMANTICS zum Zugriff auf Dateien und Verzeichnisse verwenden soll. Der Standardwert ist `false`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Rohmodus für die Textextraktion, falls möglich, verwendet wird. Der Standardwert ist `false`. Der Rohmodus kann die Indizierungsgeschwindigkeit erheblich steigern, aber der Normalmodus verbessert die Formatierung des extrahierten Textes. |

### Hinweise

**Learn more**

* [Update index](https://docs.groupdocs.com/display/searchnet/Update+index)
* [Delete indexed paths](https://docs.groupdocs.com/display/searchnet/Delete+indexed+paths)

### Siehe auch

* class [BaseOptions](../baseoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
