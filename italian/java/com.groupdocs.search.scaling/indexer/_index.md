---
title: "Indexer"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un servizio che gestisce la distribuzione dei documenti indicizzati tra i shard della rete di ricerca."
type: docs
weight: 10
url: /it/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Rappresenta un servizio che gestisce la distribuzione dei documenti indicizzati tra i shard della rete di ricerca.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Esegue l'operazione di indicizzazione. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Esegue l'operazione di indicizzazione. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Elimina i documenti indicizzati. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Riduce al minimo il numero di segmenti dell'indice unendoli uno con l'altro. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Sincronizza l'elenco dei documenti indicizzati con quelli sui shards. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Applica il batch specificato di modifiche agli attributi ai documenti indicizzati senza reindicizzazione. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Ottiene tutti gli attributi associati al documento indicizzato specificato. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Ottiene un dizionario dallo shard specificato. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Ottiene il dizionario alfabetico. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Ottiene il dizionario degli alias. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Ottiene il dizionario di sostituzione dei caratteri. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Ottiene il dizionario dei sinonimi. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Ottiene il dizionario degli omofoni. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Ottiene il dizionario del correttore ortografico. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Ottiene il dizionario delle parole stop. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Recupera il dizionario delle password. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Imposta un dizionario nello shard specificato. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Imposta un dizionario in tutti gli shard. |
|
|  | [deleteAllData()](#deleteAllData--) | Elimina tutti i dati indicizzati da tutti gli shard della rete di ricerca. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Esegue l'operazione di indicizzazione. È supportata l'indicizzazione solo da flusso e struttura.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | I documenti dal file system, dal flusso o dalla struttura. |
|
|  | password | java.lang.String[] | Le password del documento. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Le opzioni di aggiunta. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Esegue l'operazione di indicizzazione. Aggiunge i dati estratti alla rete di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | I dati estratti. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Le opzioni di indicizzazione. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Elimina i documenti indicizzati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | Le chiavi dei documenti aggiunti da flussi o strutture. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | Le opzioni di eliminazione. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Riduce il numero di segmenti dell'indice unendoli uno con l'altro. Questa operazione migliora le prestazioni di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | Le opzioni di ottimizzazione. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Sincronizza l'elenco dei documenti indicizzati con quelli sugli shard. Questa operazione risolve i problemi di indicizzazione e cancellazione dei documenti derivanti da problemi di comunicazione con i nodi della rete di ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | Le opzioni di sincronizzazione. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Applica il batch specificato di modifiche agli attributi ai documenti indicizzati senza reindicizzazione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Il batch di modifiche degli attributi. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | Le opzioni di modifica degli attributi. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Ottiene tutti gli attributi associati al documento indicizzato specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentKey | java.lang.String | La chiave del documento. |
|

**Returns:**
java.lang.String[] - Gli attributi associati al documento indicizzato specificato.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Ottiene un dizionario dallo shard specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | Il tipo di dizionario. |
|
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Ottiene il dizionario alfabetico.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Ottiene il dizionario degli alias.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Ottiene il dizionario di sostituzione dei caratteri.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Ottiene il dizionario dei sinonimi.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Ottiene il dizionario degli omofoni.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Ottiene il dizionario del correttore ortografico.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Ottiene il dizionario delle parole stop.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Recupera il dizionario delle password.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | shardIndex | int | L'indice dello shard. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Imposta un dizionario nello shard specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Il dizionario. |
|
|  | shardIndex | int | L'indice dello shard. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Imposta un dizionario in tutti gli shard.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Il dizionario. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Elimina tutti i dati indicizzati da tutti gli shard della rete di ricerca.


