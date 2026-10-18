---
title: "Ajouter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Ajoute la paire spécifiée d'alias et de texte associé à cette instance du AliasDictionarygroupdocs.search.dictionaries/aliasdictionary."
type: docs
weight: 30
url: /fr/net/groupdocs.search.dictionaries/aliasdictionary/add/
---
## AliasDictionary.Add method

Ajoute la paire spécifiée d'alias et de texte associé à cette instance du [`AliasDictionary`](../../aliasdictionary).

```csharp
public void Add(string alias, string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| alias | String | L'alias à ajouter au dictionnaire. |
| texte | String | Le texte à associer à l'alias. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lancée lorsque *alias* ou *text* est `null`. |
| ArgumentException | L'alias contient un caractère qui ne provient pas des plages a-b et 0-9. |

### Voir aussi

* class [AliasDictionary](../../aliasdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
