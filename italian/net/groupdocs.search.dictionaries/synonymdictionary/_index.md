---
title: "SynonymDictionary"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un dizionario di sinonimi."
type: docs
weight: 510
url: /it/net/groupdocs.search.dictionaries/synonymdictionary/
---
## SynonymDictionary class

Rappresenta un dizionario di sinonimi.

```csharp
public class SynonymDictionary : DictionaryBase, IEnumerable<string>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/synonymdictionary/count) { get; } | Restituisce il numero di parole contenute in questo [`SynonymDictionary`](../synonymdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/synonymdictionary/dictionarytype) { get; } | Ottiene il tipo di dizionario. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/synonymdictionary/addrange#addrange)(IEnumerable&lt;string[]&gt;) | Aggiunge la collezione specificata di gruppi di sinonimi a questa istanza del [`SynonymDictionary`](../synonymdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/synonymdictionary/addrange#addrange_1)(string[][]) | Aggiunge la collezione specificata di gruppi di sinonimi a questa istanza del [`SynonymDictionary`](../synonymdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/synonymdictionary/clear)() | Rimuove tutte le parole da questo oggetto [`SynonymDictionary`](../synonymdictionary). |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Esporta il dizionario in un file con il nome specificato. |
| [GetAllSynonymGroups](../../groupdocs.search.dictionaries/synonymdictionary/getallsynonymgroups)() | Ottiene tutti i gruppi di sinonimi contenuti in questo dizionario. |
| [GetEnumerator](../../groupdocs.search.dictionaries/synonymdictionary/getenumerator)() | Restituisce un enumeratore che itera attraverso la collezione. |
| [GetSynonymGroups](../../groupdocs.search.dictionaries/synonymdictionary/getsynonymgroups)(string) | Ottiene tutti i gruppi di sinonimi a cui appartiene la parola specificata. |
| [GetSynonyms](../../groupdocs.search.dictionaries/synonymdictionary/getsynonyms)(string) | Ottiene i sinonimi per la parola specificata. L'array risultante non contiene la parola originale. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importa un dizionario dal file specificato. |

### Osservazioni

**Learn more**

* [Synonym search](https://docs.groupdocs.com/display/searchnet/Synonym+search)
* [Managing synonym dictionary](https://docs.groupdocs.com/display/searchnet/Synonym+dictionary)

### Vedi anche

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
