---
title: "StopWordDictionary"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un dizionario di parole stop."
type: docs
weight: 500
url: /it/net/groupdocs.search.dictionaries/stopworddictionary/
---
## StopWordDictionary class

Rappresenta un dizionario di parole stop.

```csharp
public class StopWordDictionary : DictionaryBase, IEnumerable<string>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/stopworddictionary/count) { get; } | Restituisce il numero di parole di stop contenute nel [`StopWordDictionary`](../stopworddictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/stopworddictionary/dictionarytype) { get; } | Ottiene il tipo di dizionario. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/stopworddictionary/addrange#addrange)(IEnumerable&lt;string&gt;) | Aggiunge la collezione specificata di parole a questa istanza del [`StopWordDictionary`](../stopworddictionary). |
| [AddRange](../../groupdocs.search.dictionaries/stopworddictionary/addrange#addrange_1)(string[]) | Aggiunge la collezione specificata di parole a questa istanza del [`StopWordDictionary`](../stopworddictionary). |
| override [Clear](../../groupdocs.search.dictionaries/stopworddictionary/clear)() | Rimuove tutte le parole da un oggetto [`StopWordDictionary`](../stopworddictionary). |
| [Contains](../../groupdocs.search.dictionaries/stopworddictionary/contains)(string) | Determina se un oggetto [`StopWordDictionary`](../stopworddictionary) contiene la parola specificata. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Esporta il dizionario in un file con il nome specificato. |
| [GetEnumerator](../../groupdocs.search.dictionaries/stopworddictionary/getenumerator)() | Restituisce un enumeratore che itera attraverso la collezione. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importa un dizionario dal file specificato. |
| [RemoveRange](../../groupdocs.search.dictionaries/stopworddictionary/removerange#removerange)(IEnumerable&lt;string&gt;) | Rimuove la collezione specificata di parole da questa istanza del [`StopWordDictionary`](../stopworddictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/stopworddictionary/removerange#removerange_1)(string[]) | Rimuove la collezione specificata di parole da questa istanza del [`StopWordDictionary`](../stopworddictionary). |

### Osservazioni

**Learn more**

* [Indexing with stop words](https://docs.groupdocs.com/display/searchnet/Indexing+with+stop+words)
* [Managing stop word dictionary](https://docs.groupdocs.com/display/searchnet/Stop+word+dictionary)

### Vedi anche

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
