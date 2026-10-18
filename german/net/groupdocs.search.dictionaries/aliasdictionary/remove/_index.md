---
title: "Entfernen"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Entfernt den angegebenen Alias aus einem AliasDictionarygroupdocs.search.dictionaries/aliasdictionary-Objekt."
type: docs
weight: 90
url: /de/net/groupdocs.search.dictionaries/aliasdictionary/remove/
---
## AliasDictionary.Remove method

Entfernt den angegebenen Alias aus einem [`AliasDictionary`](../../aliasdictionary)-Objekt.

```csharp
public bool Remove(string alias)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Alias | String | Der zu entfernende Alias. |

### Rückgabewert

Diese Methode gibt `true` zurück, wenn der Alias erfolgreich gefunden und entfernt wurde. Diese Methode gibt `false` zurück, wenn der Alias im [`AliasDictionary`](../../aliasdictionary)-Objekt nicht gefunden wird.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wird ausgelöst, wenn *alias* `null` ist. |

### Siehe auch

* class [AliasDictionary](../../aliasdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
