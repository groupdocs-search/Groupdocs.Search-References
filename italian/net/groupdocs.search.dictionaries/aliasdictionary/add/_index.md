---
title: "Add"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Aggiunge la coppia specificata di alias e testo associato a questa istanza di AliasDictionarygroupdocs.search.dictionaries/aliasdictionary."
type: docs
weight: 30
url: /it/net/groupdocs.search.dictionaries/aliasdictionary/add/
---
## AliasDictionary.Add method

Aggiunge la coppia specificata di alias e testo associato a questa istanza di [`AliasDictionary`](../../aliasdictionary).

```csharp
public void Add(string alias, string text)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| alias | String | L'alias da aggiungere al dizionario. |
| testo | String | Il testo da associare all'alias. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Generato quando *alias* o *text* è `null`. |
| ArgumentException | L'alias contiene un carattere che non è compreso negli intervalli a-b e 0-9. |

### Vedi anche

* class [AliasDictionary](../../aliasdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
