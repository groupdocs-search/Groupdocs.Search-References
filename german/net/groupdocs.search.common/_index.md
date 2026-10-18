---
title: "GroupDocs.Search.Common"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Der Namespace stellt allgemeine Klassen der Bibliothek bereit."
type: docs
weight: 20
url: /de/net/groupdocs.search.common/
---
Der Namespace stellt allgemeine Klassen der Bibliothek bereit.

## Klassen

| Klasse | Beschreibung |
| --- | --- |
| [AttributeChangeBatch](./attributechangebatch) | Stellt einen Container für Attributänderungen dar. |
| [Cancellation](./cancellation) | Stellt ein Objekt zum Anfordern des Abbruchs einer Operation dar. |
| [ChunkSearchToken](./chunksearchtoken) | Stellt ein Token für die Fortsetzung der Chunk‑Suche (Suche nach Seiten) dar. |
| [CustomExtractorCollection](./customextractorcollection) | Enthält eine Sammlung benutzerdefinierter Extraktoren. Wenn die Sammlung einen Extraktor für eine Dateierweiterung enthält, die von integrierten Extraktoren abgedeckt wird, wird dieser Extraktor anstelle des integrierten verwendet. |
| [Document](./document) | Stellt die Basisklasse für Dokumente dar, die aus Dateisystem, Stream oder Struktur zu einem Index hinzugefügt werden. Enthält statische Methoden zum Erstellen von Dokumenten aus verschiedenen Quelltypen. |
| [DocumentField](./documentfield) | Stellt Daten eines Dokumentfeldes dar. |
| [DocumentImage](./documentimage) | Stellt Bilddaten eines Dokuments dar. |
| [Encodings](./encodings) | Enthält Namen möglicher Kodierungen. |
| [ExtractedData](./extracteddata) | Stellt Daten dar, die aus einem Dokument abgerufen und für die Indizierung aufbereitet wurden. |
| [ExtractedItemInfo](./extractediteminfo) | Stellt Informationen zu einem Container-Element dar. |
| [ExtractorSettings](./extractorsettings) | Enthält Einstellungen für den Dokumentdaten-Extraktor. |
| [FileLogger](./filelogger) | Stellt einen Logger dar, der Ereignisse und Fehler in eine lokale Datei protokolliert. |
| [FileOutputAdapter](./fileoutputadapter) | Stellt einen Ausgabeadapter dar, der Ausgaben in einer Datei sammelt. |
| [FragmentContainer](./fragmentcontainer) | Stellt einen Container für Textfragmente mit hervorgehobenen gefundenen Begriffen eines Dokumentfeldes dar. |
| [ImageFrame](./imageframe) | Stellt einen Bildrahmen dar. |
| [IndexInfo](./indexinfo) | Enthält grundlegende Informationen zu einem Index. |
| [IndexingReport](./indexingreport) | Stellt detaillierte Informationen zu einem Indexierungsvorgang dar. |
| [Notification](./notification) | Die Basisklasse für alle Benachrichtigungen an den Index. Diese Klasse enthält außerdem Methoden zum Erstellen von Benachrichtigungsobjekten. |
| [OutputAdapter](./outputadapter) | Stellt die Basisklasse eines Ausgabeadapters dar, der verwendet wird, um eine Ausgabe in einer verallgemeinerten Form zu sammeln. Die derzeit verfügbaren Adapter sind [`FileOutputAdapter`](../groupdocs.search.common/fileoutputadapter), [`StreamOutputAdapter`](../groupdocs.search.common/streamoutputadapter), [`StructureOutputAdapter`](../groupdocs.search.common/structureoutputadapter) und [`StringOutputAdapter`](../groupdocs.search.common/stringoutputadapter). |
| [ResultBuilderFactory](./resultbuilderfactory) | Stellt die Basisklasse einer Ergebnis-Builder-Fabrik dar. |
| [SearchImage](./searchimage) | Stellt ein zu suchendes Bild dar. |
| [SearchReport](./searchreport) | Stellt detaillierte Informationen zu einem Suchvorgang dar. |
| [StreamOutputAdapter](./streamoutputadapter) | Stellt einen Ausgabeadapter dar, der Ausgaben in einen Stream sammelt. |
| [StringOutputAdapter](./stringoutputadapter) | Stellt einen Ausgabeadapter dar, der Ausgaben als Zeichenkette sammelt. |
| [StructureOutputAdapter](./structureoutputadapter) | Stellt einen Ausgabeadapter dar, der Ausgaben als Struktur sammelt, die jedes Feld separat enthält. |
| [WordPattern](./wordpattern) | Stellt ein Wortmuster dar, das bei der Wortplatzhalter-Suche verwendet wird. |
## Schnittstellen

| Schnittstelle | Beschreibung |
| --- | --- |
| [IContainerItemExtractor](./icontaineritemextractor) | Stellt Methoden zum Extrahieren von Elementen aus Containerdokumenten bereit. |
| [IDocumentLoader](./idocumentloader) | Definiert die Schnittstelle des Dokumentenladers, die zum Laden von Lazy-Dokumenten verwendet wird. |
| [IFieldExtractor](./ifieldextractor) | Stellt Methoden zum Extrahieren von Feldern aus einem Dokument bereit. |
| [ILogger](./ilogger) | Definiert die Schnittstelle eines Loggers, der zum Protokollieren von Ereignissen und Fehlern in einem Index verwendet wird. |
| [IWordSplitter](./iwordsplitter) | Definiert eine Methode zum Aufteilen von Text in einzelne Wörter. |
## Aufzählung

| Aufzählung | Beschreibung |
| --- | --- |
| [DocumentSourceKind](./documentsourcekind) | Definiert die Arten von Dokumentquellen. |
| [DocumentStatus](./documentstatus) | Stellt einen Dokumentverarbeitungsstatus dar. |
| [IndexStatus](./indexstatus) | Gibt einen Indexstatus an. |
| [VersionUpdateResult](./versionupdateresult) | Stellt das Ergebnis einer Indexversions-Update-Operation dar. |

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
