---
title: "AddRange"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Aggiunge la collezione specificata di gruppi di omofoni a questa istanza di HomophoneDictionarygroupdocs.search.dictionaries/homophonedictionary."
type: docs
weight: 30
url: /it/net/groupdocs.search.dictionaries/homophonedictionary/addrange/
---
## AddRange(IEnumerable&lt;string[]&gt;) {#addrange}

Aggiunge la collezione specificata di gruppi di omofoni a questa istanza di [`HomophoneDictionary`](../../homophonedictionary).

```csharp
public void AddRange(IEnumerable<string[]> homophones)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| omofoni | IEnumerable`1 | La collezione di gruppi di omofoni da aggiungere al dizionario. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Generata quando *homophones* è `null`. |
| ArgumentException | Generata quando il numero di omofoni in un gruppo è inferiore a 2. |

### Vedi anche

* class [HomophoneDictionary](../../homophonedictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

---

## AddRange(string[][]) {#addrange_1}

Aggiunge la collezione specificata di gruppi di omofoni a questa istanza di [`HomophoneDictionary`](../../homophonedictionary).

```csharp
public void AddRange(string[][] homophones)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| omofoni | String[][] | La collezione di gruppi di omofoni da aggiungere al dizionario. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Generata quando *homophones* è `null`. |
| ArgumentException | Generata quando il numero di omofoni in un gruppo è inferiore a 2. |

### Vedi anche

* class [HomophoneDictionary](../../homophonedictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
