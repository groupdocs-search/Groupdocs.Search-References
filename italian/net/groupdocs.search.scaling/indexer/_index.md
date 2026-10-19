---
title: "Indexer"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un servizio che gestisce la distribuzione dei documenti indicizzati tra i frammenti della rete di ricerca."
type: docs
weight: 1480
url: /it/net/groupdocs.search.scaling/indexer/
---
## Indexer class

Rappresenta un servizio che gestisce la distribuzione dei documenti indicizzati tra i frammenti della rete di ricerca.

```csharp
public sealed class Indexer
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Status](../../groupdocs.search.scaling/indexer/status) { get; } | Ottiene lo stato corrente della rete di ricerca. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../groupdocs.search.scaling/indexer/add#add_1)(IList&lt;ExtractedData&gt;, IndexingOptions) | Esegue l'operazione di indicizzazione. Aggiunge i dati estratti alla rete di ricerca. |
| [Add](../../groupdocs.search.scaling/indexer/add#add)(IList&lt;Document&gt;, IList&lt;string&gt;, IndexingOptions) | Esegue l'operazione di indicizzazione. È supportata l'indicizzazione solo da flusso e struttura. |
| [ChangeAttributes](../../groupdocs.search.scaling/indexer/changeattributes)(AttributeChangeBatch, ChangeAttributesOptions) | Applica il batch specificato di modifiche agli attributi ai documenti indicizzati senza reindicizzare. |
| [Delete](../../groupdocs.search.scaling/indexer/delete)(string[], DeleteOptions) | Elimina i documenti indicizzati. |
| [DeleteAllData](../../groupdocs.search.scaling/indexer/deletealldata)() | Elimina tutti i dati indicizzati da tutti gli shard della rete di ricerca. |
| [Extract](../../groupdocs.search.scaling/indexer/extract)(IList&lt;Document&gt;, IList&lt;string&gt;, IndexingOptions) | Estrae dati dai documenti. |
| [GetAliasDictionary](../../groupdocs.search.scaling/indexer/getaliasdictionary)(int) | Ottiene il dizionario degli alias. |
| [GetAlphabet](../../groupdocs.search.scaling/indexer/getalphabet)(int) | Ottiene il dizionario dell'alfabeto. |
| [GetAttributes](../../groupdocs.search.scaling/indexer/getattributes)(string) | Ottiene tutti gli attributi associati al documento indicizzato specificato. |
| [GetCharacterReplacementDictionary](../../groupdocs.search.scaling/indexer/getcharacterreplacementdictionary)(int) | Ottiene il dizionario di sostituzione dei caratteri. |
| [GetDictionary](../../groupdocs.search.scaling/indexer/getdictionary)(DictionaryType, int) | Ottiene un dizionario dallo shard specificato. |
| [GetHomophoneDictionary](../../groupdocs.search.scaling/indexer/gethomophonedictionary)(int) | Ottiene il dizionario degli omofoni. |
| [GetPasswordDictionary](../../groupdocs.search.scaling/indexer/getpassworddictionary)(int) | Ottiene il dizionario delle password. |
| [GetSpellingCorrector](../../groupdocs.search.scaling/indexer/getspellingcorrector)(int) | Ottiene il dizionario del correttore ortografico. |
| [GetStopWordDictionary](../../groupdocs.search.scaling/indexer/getstopworddictionary)(int) | Ottiene il dizionario delle parole stop. |
| [GetSynonymDictionary](../../groupdocs.search.scaling/indexer/getsynonymdictionary)(int) | Ottiene il dizionario dei sinonimi. |
| [GetTokenizationDictionary](../../groupdocs.search.scaling/indexer/gettokenizationdictionary)(int) | Ottiene il dizionario di tokenizzazione. |
| [Optimize](../../groupdocs.search.scaling/indexer/optimize)(OptimizeOptions) | Riduce il numero di segmenti dell'indice unendoli tra loro. Questa operazione migliora le prestazioni della ricerca. |
| [SetDictionary](../../groupdocs.search.scaling/indexer/setdictionary#setdictionary)(DictionaryBase) | Imposta un dizionario in tutti gli shard. |
| [SetDictionary](../../groupdocs.search.scaling/indexer/setdictionary#setdictionary_1)(DictionaryBase, int) | Imposta un dizionario nello shard specificato. |
| [Synchronize](../../groupdocs.search.scaling/indexer/synchronize)(SynchronizeOptions) | Sincronizza l'elenco dei documenti indicizzati con quelli sugli shard. Questa operazione risolve i problemi di indicizzazione e cancellazione dei documenti derivanti da problemi di comunicazione con i nodi della rete di ricerca. |

### Vedi anche

* namespace [GroupDocs.Search.Scaling](../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
