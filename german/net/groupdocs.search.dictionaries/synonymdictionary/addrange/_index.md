---
title: "AddRange"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Fügt die angegebene Sammlung von Synonymgruppen zu dieser Instanz des SynonymDictionarygroupdocs.search.dictionaries/synonymdictionary hinzu."
type: docs
weight: 30
url: /de/net/groupdocs.search.dictionaries/synonymdictionary/addrange/
---
## AddRange(IEnumerable&lt;string[]&gt;) {#addrange}

Fügt die angegebene Sammlung von Synonymgruppen zu dieser Instanz des [`SynonymDictionary`](../../synonymdictionary) hinzu.

```csharp
public void AddRange(IEnumerable<string[]> synonyms)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Synonyme | IEnumerable`1 | Die Sammlung von Synonymgruppen, die dem Wörterbuch hinzugefügt werden soll. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wird ausgelöst, wenn *synonyms* `null` ist. |
| ArgumentException | Wird ausgelöst, wenn die Anzahl der Synonyme in einer Gruppe weniger als 2 beträgt. |

### Siehe auch

* class [SynonymDictionary](../../synonymdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

---

## AddRange(string[][]) {#addrange_1}

Fügt die angegebene Sammlung von Synonymgruppen zu dieser Instanz des [`SynonymDictionary`](../../synonymdictionary) hinzu.

```csharp
public void AddRange(string[][] synonyms)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Synonyme | String[][] | Die Sammlung von Synonymgruppen, die dem Wörterbuch hinzugefügt werden soll. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wird ausgelöst, wenn *synonyms* `null` ist. |
| ArgumentException | Wird ausgelöst, wenn die Anzahl der Synonyme in einer Gruppe weniger als 2 beträgt. |

### Siehe auch

* class [SynonymDictionary](../../synonymdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
