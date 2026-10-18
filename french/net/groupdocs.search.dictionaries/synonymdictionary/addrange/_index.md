---
title: "AddRange"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Ajoute la collection spécifiée de groupes de synonymes à cette instance du SynonymDictionarygroupdocs.search.dictionaries/synonymdictionary."
type: docs
weight: 30
url: /fr/net/groupdocs.search.dictionaries/synonymdictionary/addrange/
---
## AddRange(IEnumerable&lt;string[]&gt;) {#addrange}

Ajoute la collection spécifiée de groupes de synonymes à cette instance du [`SynonymDictionary`](../../synonymdictionary).

```csharp
public void AddRange(IEnumerable<string[]> synonyms)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| synonymes | IEnumerable`1 | La collection de groupes de synonymes à ajouter au dictionnaire. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lancée lorsque *synonyms* est `null`. |
| ArgumentException | Lancée lorsque le nombre de synonymes dans un groupe est inférieur à 2. |

### Voir aussi

* class [SynonymDictionary](../../synonymdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

---

## AddRange(string[][]) {#addrange_1}

Ajoute la collection spécifiée de groupes de synonymes à cette instance du [`SynonymDictionary`](../../synonymdictionary).

```csharp
public void AddRange(string[][] synonyms)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| synonymes | String[][] | La collection de groupes de synonymes à ajouter au dictionnaire. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lancée lorsque *synonyms* est `null`. |
| ArgumentException | Lancée lorsque le nombre de synonymes dans un groupe est inférieur à 2. |

### Voir aussi

* class [SynonymDictionary](../../synonymdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
