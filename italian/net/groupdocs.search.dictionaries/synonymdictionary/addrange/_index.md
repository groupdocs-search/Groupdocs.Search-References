---
title: "AddRange"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Aggiunge la collezione specificata di gruppi di sinonimi a questa istanza di SynonymDictionarygroupdocs.search.dictionaries/synonymdictionary."
type: docs
weight: 30
url: /it/net/groupdocs.search.dictionaries/synonymdictionary/addrange/
---
## AddRange(IEnumerable&lt;string[]&gt;) {#addrange}

Aggiunge la collezione specificata di gruppi di sinonimi a questa istanza di [`SynonymDictionary`](../../synonymdictionary).

```csharp
public void AddRange(IEnumerable<string[]> synonyms)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| sinonimi | IEnumerable`1 | La collezione di gruppi di sinonimi da aggiungere al dizionario. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Generato quando *synonyms* è `null`. |
| ArgumentException | Generato quando il numero di sinonimi in un gruppo è inferiore a 2. |

### Vedi anche

* class [SynonymDictionary](../../synonymdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

---

## AddRange(string[][]) {#addrange_1}

Aggiunge la collezione specificata di gruppi di sinonimi a questa istanza di [`SynonymDictionary`](../../synonymdictionary).

```csharp
public void AddRange(string[][] synonyms)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| sinonimi | String[][] | La collezione di gruppi di sinonimi da aggiungere al dizionario. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Generato quando *synonyms* è `null`. |
| ArgumentException | Generato quando il numero di sinonimi in un gruppo è inferiore a 2. |

### Vedi anche

* class [SynonymDictionary](../../synonymdictionary)
* namespace [GroupDocs.Search.Dictionaries](../../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
