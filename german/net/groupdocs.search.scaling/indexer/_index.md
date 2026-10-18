---
title: "Indexer"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Dienst dar, der die Verteilung von indizierten Dokumenten über die Shards des Suchnetzwerks verwaltet."
type: docs
weight: 1480
url: /de/net/groupdocs.search.scaling/indexer/
---
## Indexer class

Stellt einen Dienst dar, der die Verteilung von indizierten Dokumenten über die Shards des Suchnetzwerks verwaltet.

```csharp
public sealed class Indexer
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Status](../../groupdocs.search.scaling/indexer/status) { get; } | Ermittelt den aktuellen Status des Suchnetzwerks. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../groupdocs.search.scaling/indexer/add#add_1)(IList&lt;ExtractedData&gt;, IndexingOptions) | Führt einen Indexierungsvorgang aus. Fügt die extrahierten Daten dem Suchnetzwerk hinzu. |
| [Add](../../groupdocs.search.scaling/indexer/add#add)(IList&lt;Document&gt;, IList&lt;string&gt;, IndexingOptions) | Führt einen Indexierungsvorgang aus. Nur das Indexieren von Stream und Struktur wird unterstützt. |
| [ChangeAttributes](../../groupdocs.search.scaling/indexer/changeattributes)(AttributeChangeBatch, ChangeAttributesOptions) | Wendet die angegebene Charge von Attributänderungen auf indizierte Dokumente an, ohne neu zu indexieren. |
| [Delete](../../groupdocs.search.scaling/indexer/delete)(string[], DeleteOptions) | Löscht indizierte Dokumente. |
| [DeleteAllData](../../groupdocs.search.scaling/indexer/deletealldata)() | Löscht alle indizierten Daten von allen Shards des Suchnetzwerks. |
| [Extract](../../groupdocs.search.scaling/indexer/extract)(IList&lt;Document&gt;, IList&lt;string&gt;, IndexingOptions) | Extrahiert Daten aus Dokumenten. |
| [GetAliasDictionary](../../groupdocs.search.scaling/indexer/getaliasdictionary)(int) | Liest das Alias-Wörterbuch. |
| [GetAlphabet](../../groupdocs.search.scaling/indexer/getalphabet)(int) | Liest das Alphabet-Wörterbuch. |
| [GetAttributes](../../groupdocs.search.scaling/indexer/getattributes)(string) | Ruft alle Attribute ab, die dem angegebenen indexierten Dokument zugeordnet sind. |
| [GetCharacterReplacementDictionary](../../groupdocs.search.scaling/indexer/getcharacterreplacementdictionary)(int) | Liest das Zeichenersetzungs-Wörterbuch. |
| [GetDictionary](../../groupdocs.search.scaling/indexer/getdictionary)(DictionaryType, int) | Liest ein Wörterbuch vom angegebenen Shard. |
| [GetHomophoneDictionary](../../groupdocs.search.scaling/indexer/gethomophonedictionary)(int) | Liest das Homophon-Wörterbuch. |
| [GetPasswordDictionary](../../groupdocs.search.scaling/indexer/getpassworddictionary)(int) | Liest das Passwort-Wörterbuch. |
| [GetSpellingCorrector](../../groupdocs.search.scaling/indexer/getspellingcorrector)(int) | Liest das Rechtschreibkorrektur-Wörterbuch. |
| [GetStopWordDictionary](../../groupdocs.search.scaling/indexer/getstopworddictionary)(int) | Liest das Stoppwort-Wörterbuch. |
| [GetSynonymDictionary](../../groupdocs.search.scaling/indexer/getsynonymdictionary)(int) | Liest das Synonym-Wörterbuch. |
| [GetTokenizationDictionary](../../groupdocs.search.scaling/indexer/gettokenizationdictionary)(int) | Liest das Tokenisierungs-Wörterbuch. |
| [Optimize](../../groupdocs.search.scaling/indexer/optimize)(OptimizeOptions) | Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. Dieser Vorgang verbessert die Suchleistung. |
| [SetDictionary](../../groupdocs.search.scaling/indexer/setdictionary#setdictionary)(DictionaryBase) | Setzt ein Wörterbuch in allen Shards. |
| [SetDictionary](../../groupdocs.search.scaling/indexer/setdictionary#setdictionary_1)(DictionaryBase, int) | Setzt ein Wörterbuch im angegebenen Shard. |
| [Synchronize](../../groupdocs.search.scaling/indexer/synchronize)(SynchronizeOptions) | Synchronisiert die Liste der indizierten Dokumente mit denen auf den Shards. Dieser Vorgang behebt Probleme beim Indexieren und Löschen von Dokumenten, die durch Kommunikationsprobleme mit den Knoten des Suchnetzwerks entstanden sind. |

### Siehe auch

* namespace [GroupDocs.Search.Scaling](../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
