---
title: "AddRange"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Fügt die angegebene Sammlung von Homophon‑Gruppen zu dieser Instanz des HomophoneDictionarygroupdocs.search.dictionaries/homophonedictionary hinzu."
type: docs
weight: 30
url: /de/net/groupdocs.search.dictionaries/homophonedictionary/addrange/
---
## AddRange(IEnumerable&lt;string[]&gt;) {#addrange}

Fügt die angegebene Sammlung von Homophon‑Gruppen zu dieser Instanz des [`HomophoneDictionary`](../../homophonedictionary) hinzu.

```csharp
public void AddRange(IEnumerable<string[]> homophones)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Homophone | IEnumerable`1 | Die Sammlung von Homophon‑Gruppen, die dem Wörterbuch hinzugefügt werden soll. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wird ausgelöst, wenn *homophones* `null` ist. |
| ArgumentException | Wird ausgelöst, wenn die Anzahl der Homophone in einer Gruppe weniger als 2 beträgt. |

### Siehe auch

* class [HomophoneDictionary](../../homophonedictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

---

## AddRange(string[][]) {#addrange_1}

Fügt die angegebene Sammlung von Homophon‑Gruppen zu dieser Instanz des [`HomophoneDictionary`](../../homophonedictionary) hinzu.

```csharp
public void AddRange(string[][] homophones)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Homophone | String[][] | Die Sammlung von Homophon‑Gruppen, die dem Wörterbuch hinzugefügt werden soll. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wird ausgelöst, wenn *homophones* `null` ist. |
| ArgumentException | Wird ausgelöst, wenn die Anzahl der Homophone in einer Gruppe weniger als 2 beträgt. |

### Siehe auch

* class [HomophoneDictionary](../../homophonedictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
