---
title: "Indexer"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een service voor die de distributie van geïndexeerde documenten over shards van het zoeknetwerk beheert."
type: docs
weight: 10
url: /nl/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Stelt een service voor die de distributie van geïndexeerde documenten over shards van het zoeknetwerk beheert.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Voert een indexeerbewerking uit. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Voert een indexeerbewerking uit. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Verwijdert geïndexeerde documenten. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Minimaliseert het aantal indexsegmenten door ze één voor één samen te voegen. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Synchroniseert de lijst met geïndexeerde documenten met die op shards. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Past de opgegeven batch van attribuutwijzigingen toe op geïndexeerde documenten zonder opnieuw te indexeren. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Haalt alle attributen op die geassocieerd zijn met het opgegeven geïndexeerde document. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Haalt een woordenboek op van de opgegeven shard. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Haalt het alfabetwoordenboek op. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Haalt het aliaswoordenboek op. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Haalt het tekenvervangingswoordenboek op. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Haalt het synoniemenwoordenboek op. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Haalt het homofoonwoordenboek op. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Haalt het spellingcorrectiewoordenboek op. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Haalt het stopwoordenwoordenboek op. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Haalt het wachtwoordwoordenboek op. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Stelt een woordenboek in op de opgegeven shard. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Stelt een woordenboek in op alle shards. |
|
|  | [deleteAllData()](#deleteAllData--) | Verwijdert alle geïndexeerde gegevens van alle shards van het zoeknetwerk. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Voert een indexeerbewerking uit. Indexeren alleen vanaf stream en structuur wordt ondersteund.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | De documenten van het bestandssysteem, stream of structuur. |
|
|  | wachtwoorden | java.lang.String[] | De documentwachtwoorden. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | De toevoegopties. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Voert een indexeerbewerking uit. Voegt de geëxtraheerde gegevens toe aan het zoeknetwerk.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | De geëxtraheerde gegevens. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | De indexeeropties. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Verwijdert geïndexeerde documenten.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | De sleutels van documenten die zijn toegevoegd vanuit streams of structuren. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | De verwijderopties. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Minimaliseert het aantal indexsegmenten door ze één met de ander te combineren. Deze bewerking verbetert de zoekprestaties.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | De optimalisatieopties. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Synchroniseert de lijst met geïndexeerde documenten met die op shards. Deze bewerking lost problemen op met indexeren en verwijderen van documenten die voortkwamen uit communicatieproblemen met de knooppunten van het zoeknetwerk.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | De synchronisatieopties. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Past de opgegeven batch van attribuutwijzigingen toe op geïndexeerde documenten zonder opnieuw te indexeren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | De batch voor attribuutwijzigingen. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | De opties voor het wijzigen van attributen. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Haalt alle attributen op die geassocieerd zijn met het opgegeven geïndexeerde document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | documentKey | java.lang.String | De documentsleutel. |
|

**Returns:**
java.lang.String[] - De attributen die geassocieerd zijn met het opgegeven geïndexeerde document.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Haalt een woordenboek op van de opgegeven shard.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | Het type woordenboek. |
|
|  | shardIndex | int | De shard-index. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Haalt het alfabetwoordenboek op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | shardIndex | int | De shard-index. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Haalt het aliaswoordenboek op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | shardIndex | int | De shard-index. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Haalt het tekenvervangingswoordenboek op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | shardIndex | int | De shard-index. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Haalt het synoniemenwoordenboek op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | shardIndex | int | De shard-index. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Haalt het homofoonwoordenboek op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | shardIndex | int | De shard-index. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Haalt het spellingcorrectiewoordenboek op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | shardIndex | int | De shard-index. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Haalt het stopwoordenwoordenboek op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | shardIndex | int | De shard-index. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Haalt het wachtwoordwoordenboek op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | shardIndex | int | De shard-index. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Stelt een woordenboek in op de opgegeven shard.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Het woordenboek. |
|
|  | shardIndex | int | De shard-index. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Stelt een woordenboek in op alle shards.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Het woordenboek. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Verwijdert alle geïndexeerde gegevens van alle shards van het zoeknetwerk.


