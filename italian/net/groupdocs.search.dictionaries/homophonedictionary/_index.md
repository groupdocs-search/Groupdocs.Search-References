---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un dizionario di omofoni eterografici."
type: docs
weight: 460
url: /it/net/groupdocs.search.dictionaries/homophonedictionary/
---
## HomophoneDictionary class

Rappresenta un dizionario di omofoni eterografici.

```csharp
public class HomophoneDictionary : DictionaryBase, IEnumerable<string>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/homophonedictionary/count) { get; } | Ottiene il numero di parole contenute in questo [`HomophoneDictionary`](../homophonedictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/homophonedictionary/dictionarytype) { get; } | Ottiene il tipo di dizionario. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange)(IEnumerable&lt;string[]&gt;) | Aggiunge la collezione specificata di gruppi di omofoni a questa istanza di [`HomophoneDictionary`](../homophonedictionary). |
| [AddRange](../../groupdocs.search.dictionaries/homophonedictionary/addrange#addrange_1)(string[][]) | Aggiunge la collezione specificata di gruppi di omofoni a questa istanza di [`HomophoneDictionary`](../homophonedictionary). |
| override [Clear](../../groupdocs.search.dictionaries/homophonedictionary/clear)() | Rimuove tutte le parole da un oggetto [`HomophoneDictionary`](../homophonedictionary). |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Esporta il dizionario in un file con il nome specificato. |
| [GetAllHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/getallhomophonegroups)() | Ottiene tutti i gruppi di omofoni contenuti in questo dizionario. |
| [GetEnumerator](../../groupdocs.search.dictionaries/homophonedictionary/getenumerator)() | Restituisce un enumeratore che itera attraverso la collezione. |
| [GetHomophoneGroups](../../groupdocs.search.dictionaries/homophonedictionary/gethomophonegroups)(string) | Ottiene tutti i gruppi di omofoni a cui appartiene la parola specificata. |
| [GetHomophones](../../groupdocs.search.dictionaries/homophonedictionary/gethomophones)(string) | Ottiene gli omofoni per la parola specificata. L'array risultante non contiene la parola originale. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importa un dizionario dal file specificato. |

### Osservazioni

**Learn more**

* [Homophone search](https://docs.groupdocs.com/display/searchnet/Homophone+search)
* [Managing homophone dictionary](https://docs.groupdocs.com/display/searchnet/Homophone+dictionary)

### Vedi anche

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
