---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un dizionario di sostituzione dei caratteri che viene utilizzato durante il processo di indicizzazione. La sostituzione dei caratteri può essere usata, ad esempio, per rimuovere gli accenti dai caratteri accentati o per creare un indice non sensibile al maiuscolo/minuscolo."
type: docs
weight: 390
url: /it/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Rappresenta un dizionario di sostituzione dei caratteri utilizzato durante il processo di indicizzazione. La sostituzione dei caratteri può essere usata, ad esempio, per rimuovere gli accenti dai caratteri accentati o per creare un indice non sensibile al maiuscolo/minuscolo.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Ottiene il numero di punti di codice Unicode contenuti in questo [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Ottiene il tipo di dizionario. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Aggiunge la collezione specificata di sostituzioni di caratteri a questa istanza di [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Aggiunge la collezione specificata di sostituzioni di caratteri a questa istanza di [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Aggiunge la collezione specificata di sostituzioni di caratteri a questa istanza di [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Aggiunge la collezione specificata di sostituzioni di punti di codice Unicode a questa istanza di [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Rimuove tutte le sostituzioni di caratteri da un oggetto [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Determina se un oggetto [`CharacterReplacementDictionary`](../characterreplacementdictionary) contiene una sostituzione per il punto di codice Unicode specificato. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Esporta il dizionario in un file con il nome specificato. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Restituisce un enumeratore che itera attraverso la collezione. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Ottiene una sostituzione per il punto di codice Unicode specificato. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importa un dizionario dal file specificato. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Rimuove la collezione specificata di sostituzioni di caratteri da questa istanza di [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Rimuove la collezione specificata di sostituzioni di caratteri da questa istanza di [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Rimuove la collezione specificata di sostituzioni di punti di codice Unicode da questa istanza di [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Rimuove la collezione specificata di sostituzioni di punti di codice Unicode da questa istanza di [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Osservazioni

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Vedi anche

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
