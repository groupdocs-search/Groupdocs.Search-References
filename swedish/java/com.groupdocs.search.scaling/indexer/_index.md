---
title: "Indexer"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en tjänst som hanterar distributionen av indexerade dokument över söknätverkets shards."
type: docs
weight: 10
url: /sv/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Representerar en tjänst som hanterar distributionen av indexerade dokument över söknätverkets shards.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Utför indexeringsoperation. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Utför indexeringsoperation. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Raderar indexerade dokument. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Minimerar antalet indexsegment genom att slå samman dem ett med ett. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Synkroniserar listan över indexerade dokument med de på shards. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Tillämpar den angivna batchen av attributändringar på indexerade dokument utan omindexering. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Hämtar alla attribut som är associerade med det angivna indexerade dokumentet. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Hämtar en ordbok från den angivna sharden. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Hämtar alfabetordboken. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Hämtar aliasordboken. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Hämtar teckenersättningsordboken. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Hämtar synonymordboken. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Hämtar homofonordboken. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Hämtar stavningskorrigeringsordboken. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Hämtar stoppordordboken. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Hämtar lösenordsordlistan. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Ställer in en ordlista i den angivna sharden. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Ställer in en ordlista i alla shards. |
|
|  | [deleteAllData()](#deleteAllData--) | Tar bort all indexerad data från alla shards i söknätverket. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Utför indexeringsoperation. Endast indexering från ström och struktur stöds.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Dokumenten från filsystem, ström eller struktur. |
|
|  | lösenord | java.lang.String[] | Dokumentets lösenord. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Alternativen för att lägga till. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Utför indexeringsoperation. Lägger till den extraherade datan i söknätverket.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Den extraherade datan. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Indexeringsalternativen. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Raderar indexerade dokument.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | Nycklarna för dokument som lagts till från strömmar eller strukturer. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | Alternativen för borttagning. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Minimerar antalet indexsegment genom att slå ihop dem med varandra. Denna operation förbättrar sökprestanda.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | Optimeringsalternativen. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Synkroniserar listan över indexerade dokument med de på shards. Denna operation åtgärdar problem med indexering och borttagning av dokument som uppstod på grund av kommunikationsproblem med söknätverkets noder.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | Synkroniseringsalternativen. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Tillämpar den angivna batchen av attributändringar på indexerade dokument utan omindexering.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Batchen för attributändringar. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | Alternativen för att ändra attribut. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Hämtar alla attribut som är associerade med det angivna indexerade dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | documentKey | java.lang.String | Dokumentnyckeln. |
|

**Returns:**
java.lang.String[] – Attributen som är associerade med det angivna indexerade dokumentet.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Hämtar en ordbok från den angivna sharden.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | Ordlistans typ. |
|
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Hämtar alfabetordboken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Hämtar aliasordboken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Hämtar teckenersättningsordboken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Hämtar synonymordboken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Hämtar homofonordboken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Hämtar stavningskorrigeringsordboken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Hämtar stoppordordboken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Hämtar lösenordsordlistan.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | shardIndex | int | Shard-indexet. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Ställer in en ordlista i den angivna sharden.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Ordlistan. |
|
|  | shardIndex | int | Shard-indexet. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Ställer in en ordlista i alla shards.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Ordlistan. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Tar bort all indexerad data från alla shards i söknätverket.


