---
title: "PasswordDictionary"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un dizionario di password dei documenti."
type: docs
weight: 480
url: /it/net/groupdocs.search.dictionaries/passworddictionary/
---
## PasswordDictionary class

Rappresenta un dizionario di password dei documenti.

```csharp
public class PasswordDictionary : DictionaryBase, IEnumerable<string>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/passworddictionary/count) { get; } | Ottiene il numero di elementi contenuti nel dizionario. |
| override [DictionaryType](../../groupdocs.search.dictionaries/passworddictionary/dictionarytype) { get; } | Ottiene il tipo di dizionario. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../groupdocs.search.dictionaries/passworddictionary/add)(string, string) | Aggiunge una password per un documento al dizionario. |
| override [Clear](../../groupdocs.search.dictionaries/passworddictionary/clear)() | Rimuove tutte le password da questo oggetto [`PasswordDictionary`](../passworddictionary). |
| [Contains](../../groupdocs.search.dictionaries/passworddictionary/contains)(string) | Determina se il dizionario contiene una password per il documento specificato. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Esporta il dizionario in un file con il nome specificato. |
| [GetEnumerator](../../groupdocs.search.dictionaries/passworddictionary/getenumerator)() | Restituisce un enumeratore che itera attraverso la collezione. |
| [GetPassword](../../groupdocs.search.dictionaries/passworddictionary/getpassword)(string) | Ottiene la password per il file. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Importa un dizionario dal file specificato. |
| [Remove](../../groupdocs.search.dictionaries/passworddictionary/remove)(string) | Rimuove una password del documento specificato dal dizionario. |

### Osservazioni

**Learn more**

* [Indexing password protected documents](https://docs.groupdocs.com/display/searchnet/Indexing+password+protected+documents)
* [Managing document passwords](https://docs.groupdocs.com/display/searchnet/Document+passwords)

### Vedi anche

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
