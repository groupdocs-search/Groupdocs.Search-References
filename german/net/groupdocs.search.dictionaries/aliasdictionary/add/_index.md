---
title: "Hinzufügen"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Fügt das angegebene Paar aus Alias und zugehörigem Text zu dieser Instanz des AliasDictionarygroupdocs.search.dictionaries/aliasdictionary hinzu."
type: docs
weight: 30
url: /de/net/groupdocs.search.dictionaries/aliasdictionary/add/
---
## AliasDictionary.Add method

Fügt das angegebene Paar aus Alias und zugehörigem Text zu dieser Instanz des [`AliasDictionary`](../../aliasdictionary) hinzu.

```csharp
public void Add(string alias, string text)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Alias | String | Der Alias, der dem Wörterbuch hinzugefügt werden soll. |
| Text | String | Der Text, der dem Alias zugeordnet werden soll. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wird ausgelöst, wenn *alias* oder *text* `null` ist. |
| ArgumentException | Alias enthält ein Zeichen, das nicht aus den Bereichen a-b und 0-9 stammt. |

### Siehe auch

* class [AliasDictionary](../../aliasdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
