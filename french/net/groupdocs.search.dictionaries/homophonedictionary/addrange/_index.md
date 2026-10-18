---
title: "AddRange"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Ajoute la collection spécifiée de groupes d'homophones à cette instance de HomophoneDictionarygroupdocs.search.dictionaries/homophonedictionary."
type: docs
weight: 30
url: /fr/net/groupdocs.search.dictionaries/homophonedictionary/addrange/
---
## AddRange(IEnumerable&lt;string[]&gt;) {#addrange}

Ajoute la collection spécifiée de groupes d'homophones à cette instance du [`HomophoneDictionary`](../../homophonedictionary).

```csharp
public void AddRange(IEnumerable<string[]> homophones)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| homophones | IEnumerable`1 | La collection de groupes d'homophones à ajouter au dictionnaire. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lancé lorsque *homophones* est `null`. |
| ArgumentException | Lancé lorsque le nombre d'homophones dans un groupe est inférieur à 2. |

### Voir aussi

* class [HomophoneDictionary](../../homophonedictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

---

## AddRange(string[][]) {#addrange_1}

Ajoute la collection spécifiée de groupes d'homophones à cette instance du [`HomophoneDictionary`](../../homophonedictionary).

```csharp
public void AddRange(string[][] homophones)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| homophones | String[][] | La collection de groupes d'homophones à ajouter au dictionnaire. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lancé lorsque *homophones* est `null`. |
| ArgumentException | Lancé lorsque le nombre d'homophones dans un groupe est inférieur à 2. |

### Voir aussi

* class [HomophoneDictionary](../../homophonedictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
