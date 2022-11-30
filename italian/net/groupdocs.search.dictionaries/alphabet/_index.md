---
title: Alphabet
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta un dizionario di caratteri utilizzato durante lindicizzazione per rilevare il tipo di carattere. Ogni carattere può essere gestito come separatore come lettera o entrambi.
type: docs
weight: 360
url: /it/net/groupdocs.search.dictionaries/alphabet/
---
## Alphabet class

Rappresenta un dizionario di caratteri utilizzato durante l'indicizzazione per rilevare il tipo di carattere. Ogni carattere può essere gestito come separatore, come lettera o entrambi.

```csharp
public class Alphabet : DictionaryBase, IEnumerable<char>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/alphabet/count) { get; } | Ottiene il numero di caratteri contenuti nel file[`Alphabet`](../alphabet) . |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clear](../../groupdocs.search.dictionaries/alphabet/clear)() | Imposta ilSeparator digitare per tutti i caratteri in this[`Alphabet`](../alphabet) . |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Esporta il dizionario in un file con il nome specificato. |
| [GetCharacterType](../../groupdocs.search.dictionaries/alphabet/getcharactertype)(char) | Ottiene un tipo di carattere. |
| [GetEnumerator](../../groupdocs.search.dictionaries/alphabet/getenumerator)() | Restituisce un enumeratore che scorre la raccolta. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importa un dizionario dal file specificato. |
| [SetRange](../../groupdocs.search.dictionaries/alphabet/setrange)(char[], CharacterType) | Imposta il tipo per ciascun carattere della raccolta specificata in questa istanza di[`Alphabet`](../alphabet) . |

### Osservazioni

**Scopri di più**

* [Tipi di caratteri](https://docs.groupdocs.com/display/searchnet/Character+types)
* [Gestire l'alfabeto](https://docs.groupdocs.com/display/searchnet/Alphabet)

### Guarda anche

* class [DictionaryBase](../dictionarybase)
* spazio dei nomi [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->