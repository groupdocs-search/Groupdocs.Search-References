---
title: AddRange
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Aggiunge la raccolta specificata di gruppi omofoni a questa istanza diHomophoneDictionarygroupdocs.search.dictionaries/homophonedictionary .
type: docs
weight: 20
url: /it/net/groupdocs.search.dictionaries/homophonedictionary/addrange/
---
## AddRange(IEnumerable&lt;string[]&gt;) {#addrange}

Aggiunge la raccolta specificata di gruppi omofoni a questa istanza di[`HomophoneDictionary`](../../homophonedictionary) .

```csharp
public void AddRange(IEnumerable<string[]> homophones)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| homophones | IEnumerable`1 | La raccolta di gruppi omofoni da aggiungere al dizionario. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Lanciato quando*homophones* È`nullo`. |
| ArgumentException | Generato quando il numero di omofoni in un gruppo è inferiore a 2. |

### Guarda anche

* class [HomophoneDictionary](../../homophonedictionary)
* spazio dei nomi [GroupDocs.Search.Dictionaries](../../homophonedictionary)
* assemblea [GroupDocs.Search](../../../)

---

## AddRange(string[][]) {#addrange_1}

Aggiunge la raccolta specificata di gruppi omofoni a questa istanza di[`HomophoneDictionary`](../../homophonedictionary) .

```csharp
public void AddRange(string[][] homophones)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| homophones | String[][] | La raccolta di gruppi omofoni da aggiungere al dizionario. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Lanciato quando*homophones* È`nullo`. |
| ArgumentException | Generato quando il numero di omofoni in un gruppo è inferiore a 2. |

### Guarda anche

* class [HomophoneDictionary](../../homophonedictionary)
* spazio dei nomi [GroupDocs.Search.Dictionaries](../../homophonedictionary)
* assemblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
