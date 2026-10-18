---
title: "SeparateProcessOptionen"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Optionen zum Extrahieren von Daten aus Dokumenten in einem separaten Prozess bereit."
type: docs
weight: 1110
url: /de/net/groupdocs.search.options/separateprocessoptions/
---
## SeparateProcessOptions class

Stellt Optionen zum Extrahieren von Daten aus Dokumenten in einem separaten Prozess bereit.

```csharp
public class SeparateProcessOptions
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AssemblyPath](../../groupdocs.search.options/separateprocessoptions/assemblypath) { get; set; } | Liefert oder setzt den Pfad zur separaten Prozess‑Assembly. |
| [ExtractInSeparateProcess](../../groupdocs.search.options/separateprocessoptions/extractinseparateprocess) { get; set; } | Liefert oder setzt einen Wert, der angibt, ob ein separater Prozess zum Extrahieren von Daten aus Dokumenten verwendet wird. Der Standardwert ist `false`. Wenn diese Option aktiviert ist, wird die Datener extraction in einem separaten Prozess nur in einem Thread durchgeführt. Die angegebene Anzahl von Threads wird beim Extrahieren in einem separaten Prozess ignoriert. |
| [Timeout](../../groupdocs.search.options/separateprocessoptions/timeout) { get; set; } | Liefert oder setzt die maximale Wartezeit für das Ergebnis der Datenextraktion in einem separaten Prozess. Der Standardwert beträgt 10 Minuten. |
| [UseDotnetToStartProcess](../../groupdocs.search.options/separateprocessoptions/usedotnettostartprocess) { get; set; } | Liefert oder setzt das Flag für die Verwendung von `dotnet` zum Starten des Prozesses. Der Standardwert ist `true`. Setzen Sie den Wert auf `false`, wenn Sie eine eigenständige Anwendung starten möchten. Beachten Sie, dass `dotnet` beim Starten des alten .NET Frameworks niemals verwendet wird. |

### Siehe auch

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
