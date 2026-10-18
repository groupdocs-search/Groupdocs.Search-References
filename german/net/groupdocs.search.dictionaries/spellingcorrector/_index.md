---
title: "SpellingCorrector"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Rechtschreibkorrektor für Begriffe in einer Abfrage dar."
type: docs
weight: 490
url: /de/net/groupdocs.search.dictionaries/spellingcorrector/
---
## SpellingCorrector class

Stellt einen Rechtschreibkorrektor für Begriffe in einer Abfrage dar.

```csharp
public class SpellingCorrector : DictionaryBase
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/spellingcorrector/count) { get; } | Liefert die Anzahl der Wörter, die in diesem [`SpellingCorrector`](../spellingcorrector) enthalten sind. |
| override [DictionaryType](../../groupdocs.search.dictionaries/spellingcorrector/dictionarytype) { get; } | Ermittelt den Wörterbuchtyp. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/spellingcorrector/addrange#addrange)(IEnumerable&lt;string&gt;) | Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des [`SpellingCorrector`](../spellingcorrector) hinzu. |
| [AddRange](../../groupdocs.search.dictionaries/spellingcorrector/addrange#addrange_1)(string[]) | Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des [`SpellingCorrector`](../spellingcorrector) hinzu. |
| override [Clear](../../groupdocs.search.dictionaries/spellingcorrector/clear)() | Entfernt alle Wörter aus einem [`SpellingCorrector`](../spellingcorrector)-Objekt. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Exportiert das Wörterbuch in eine Datei mit dem angegebenen Namen. |
| [GetWords](../../groupdocs.search.dictionaries/spellingcorrector/getwords)() | Liefert die Sammlung von Wörtern, die derzeit in diesem [`SpellingCorrector`](../spellingcorrector) enthalten ist. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importiert ein Wörterbuch aus der angegebenen Datei. |

### Hinweise

**Learn more**

* [Spell checking](https://docs.groupdocs.com/display/searchnet/Spell+checking)
* [Managing spelling corrector](https://docs.groupdocs.com/display/searchnet/Spelling+corrector)

### Siehe auch

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
