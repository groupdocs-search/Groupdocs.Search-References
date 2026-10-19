---
title: "Alfabeto"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un dizionario di caratteri utilizzato durante l'indicizzazione per rilevare il tipo di carattere. Ogni carattere può essere gestito come separatore, come lettera o entrambi."
type: docs
weight: 380
url: /it/net/groupdocs.search.dictionaries/alphabet/
---
## Alphabet class

Rappresenta un dizionario di caratteri utilizzato durante l'indicizzazione per rilevare il tipo di carattere. Ogni carattere può essere gestito come separatore, come lettera o entrambi.

```csharp
public class Alphabet : DictionaryBase, IEnumerable<int>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/alphabet/count) { get; } | Ottiene il numero di caratteri contenuti nell'[`Alphabet`](../alphabet). |
| override [DictionaryType](../../groupdocs.search.dictionaries/alphabet/dictionarytype) { get; } | Ottiene il tipo di dizionario. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Clear](../../groupdocs.search.dictionaries/alphabet/clear)() | Imposta il tipo di Separator per tutti i caratteri in questo [`Alphabet`](../alphabet). |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Esporta il dizionario in un file con il nome specificato. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype#getcharactertype)(char) | Ottiene un tipo di carattere. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype#getcharactertype_1)(int) | Ottiene un tipo di punto di codice Unicode. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype#getcharactertype_2)(string) | Ottiene un tipo di carattere. Questo metodo può essere usato per ottenere il tipo di coppia surrogata. |
| [GetEnumerator](../../groupdocs.search.dictionaries/alphabet/getenumerator)() | Restituisce un enumeratore che itera attraverso la collezione. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importa un dizionario dal file specificato. |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange#setrange)(char[], CharacterType) | Imposta il tipo per ogni carattere della collezione specificata in questa istanza di [`Alphabet`](../alphabet). |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange#setrange_1)(int[], CharacterType) | Imposta il tipo per ogni carattere della collezione specificata in questa istanza di [`Alphabet`](../alphabet). |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange#setrange_2)(string[], CharacterType) | Imposta il tipo per ogni carattere della collezione specificata in questa istanza di [`Alphabet`](../alphabet). |

### Osservazioni

**Learn more**

* [Character types](https://docs.groupdocs.com/display/searchnet/Character+types)
* [Managing alphabet](https://docs.groupdocs.com/display/searchnet/Alphabet)

### Vedi anche

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
