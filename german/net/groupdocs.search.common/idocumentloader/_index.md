---
title: "IDocumentLoader"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Definiert die Schnittstelle des Dokumentenladers, die zum Laden von Lazy-Dokumenten verwendet wird."
type: docs
weight: 180
url: /de/net/groupdocs.search.common/idocumentloader/
---
## IDocumentLoader interface

Definiert die Schnittstelle des Dokumentenladers, die zum Laden von Lazy-Dokumenten verwendet wird.

```csharp
public interface IDocumentLoader
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CloseDocument](../../groupdocs.search.common/idocumentloader/closedocument)() | Schließt das geladene Dokument. Diese Methode wird vom Index aufgerufen, wenn er die Verarbeitung des Dokuments abgeschlossen hat. |
| [LoadDocument](../../groupdocs.search.common/idocumentloader/loaddocument)() | Lädt ein Dokument. Diese Methode wird vom Index aufgerufen, wenn er bereit ist, das Dokument zu verarbeiten. |

### Siehe auch

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
