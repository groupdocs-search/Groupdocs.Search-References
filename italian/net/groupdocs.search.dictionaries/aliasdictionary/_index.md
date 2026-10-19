---
title: "AliasDictionary"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un dizionario di alias."
type: docs
weight: 360
url: /it/net/groupdocs.search.dictionaries/aliasdictionary/
---
## AliasDictionary class

Rappresenta un dizionario di alias.

```csharp
public class AliasDictionary : DictionaryBase, IEnumerable<string>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/aliasdictionary/count) { get; } | Ottiene il numero di alias contenuti nel [`AliasDictionary`](../aliasdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/aliasdictionary/dictionarytype) { get; } | Ottiene il tipo di dizionario. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../groupdocs.search.dictionaries/aliasdictionary/add)(string, string) | Aggiunge la coppia specificata di alias e testo associato a questa istanza del [`AliasDictionary`](../aliasdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange)(AliasReplacementPair[]) | Aggiunge la collezione specificata di coppie alias/sostituzione a questa istanza del [`AliasDictionary`](../aliasdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_1)(IEnumerable&lt;AliasReplacementPair&gt;) | Aggiunge la collezione specificata di coppie alias/sostituzione a questa istanza del [`AliasDictionary`](../aliasdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/aliasdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;string, string&gt;&gt;) | Aggiunge la collezione specificata di coppie alias/sostituzione a questa istanza del [`AliasDictionary`](../aliasdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/aliasdictionary/clear)() | Rimuove tutti gli alias da un oggetto [`AliasDictionary`](../aliasdictionary). |
| [Contains](../../groupdocs.search.dictionaries/aliasdictionary/contains)(string) | Determina se un oggetto [`AliasDictionary`](../aliasdictionary) contiene l'alias specificato. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Esporta il dizionario in un file con il nome specificato. |
| [GetEnumerator](../../groupdocs.search.dictionaries/aliasdictionary/getenumerator)() | Restituisce un enumeratore che itera attraverso la collezione. |
| [GetText](../../groupdocs.search.dictionaries/aliasdictionary/gettext)(string) | Ottiene un testo associato all'alias specificato. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importa un dizionario dal file specificato. |
| [Remove](../../groupdocs.search.dictionaries/aliasdictionary/remove)(string) | Rimuove l'alias specificato da un oggetto [`AliasDictionary`](../aliasdictionary). |

### Osservazioni

**Learn more**

* [Using aliases](https://docs.groupdocs.com/display/searchnet/Using+aliases)
* [Managing alias dictionary](https://docs.groupdocs.com/display/searchnet/Alias+dictionary)

### Vedi anche

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
