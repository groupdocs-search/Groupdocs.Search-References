---
title: "Indexer"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Dienst dar, der die Verteilung indizierter Dokumente über Shards des Suchnetzwerks verwaltet."
type: docs
weight: 10
url: /de/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Stellt einen Dienst dar, der die Verteilung indizierter Dokumente über Shards des Suchnetzwerks verwaltet.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Führt einen Indexierungsvorgang aus. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Führt einen Indexierungsvorgang aus. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Löscht indizierte Dokumente. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Synchronisiert die Liste der indizierten Dokumente mit denen auf den Shards. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Wendet das angegebene Batch von Attributänderungen auf indizierte Dokumente an, ohne sie neu zu indexieren. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Ruft alle Attribute ab, die mit dem angegebenen indizierten Dokument verknüpft sind. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Liest ein Wörterbuch vom angegebenen Shard. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | Liest das Alphabet-Wörterbuch. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Liest das Alias-Wörterbuch. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Liest das Zeichenersetzungs-Wörterbuch. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Liest das Synonym-Wörterbuch. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Liest das Homophon-Wörterbuch. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Liest das Rechtschreibkorrektur-Wörterbuch. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Liest das Stoppwort-Wörterbuch. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Ruft das Passwortwörterbuch ab. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Setzt ein Wörterbuch im angegebenen Shard. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Setzt ein Wörterbuch in allen Shards. |
|
|  | [deleteAllData()](#deleteAllData--) | Löscht alle indizierten Daten aus allen Shards des Suchnetzwerks. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Führt einen Indexierungsvorgang aus. Nur das Indexieren von Stream und Struktur wird unterstützt.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Die Dokumente aus dem Dateisystem, Stream oder Struktur. |
|
|  | Passwörter | java.lang.String[] | Die Dokumentpasswörter. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Die Hinzufügungsoptionen. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


Führt einen Indexierungsvorgang aus. Fügt die extrahierten Daten dem Suchnetzwerk hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Die extrahierten Daten. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Die Indexierungsoptionen. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Löscht indizierte Dokumente.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | Die Schlüssel der aus Streams oder Strukturen hinzugefügten Dokumente. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | Die Löschoptionen. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. Dieser Vorgang verbessert die Suchleistung.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | Die Optimierungsoptionen. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Synchronisiert die Liste der indizierten Dokumente mit denen auf den Shards. Dieser Vorgang behebt Probleme beim Indexieren und Löschen von Dokumenten, die durch Kommunikationsprobleme mit den Knoten des Suchnetzwerks entstanden sind.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | Die Synchronisationsoptionen. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Wendet das angegebene Batch von Attributänderungen auf indizierte Dokumente an, ohne sie neu zu indexieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Das Batch für Attributänderungen. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | Die Optionen zum Ändern von Attributen. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Ruft alle Attribute ab, die mit dem angegebenen indizierten Dokument verknüpft sind.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | documentKey | java.lang.String | Der Dokumentenschlüssel. |
|

**Returns:**
java.lang.String[] – Die mit dem angegebenen indizierten Dokument verbundenen Attribute.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Liest ein Wörterbuch vom angegebenen Shard.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | Der Wörterbuchtyp. |
|
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Liest das Alphabet-Wörterbuch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Liest das Alias-Wörterbuch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Liest das Zeichenersetzungs-Wörterbuch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Liest das Synonym-Wörterbuch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Liest das Homophon-Wörterbuch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Liest das Rechtschreibkorrektur-Wörterbuch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Liest das Stoppwort-Wörterbuch.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Ruft das Passwortwörterbuch ab.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | shardIndex | int | Der Shard-Index. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Setzt ein Wörterbuch im angegebenen Shard.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Das Wörterbuch. |
|
|  | shardIndex | int | Der Shard-Index. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Setzt ein Wörterbuch in allen Shards.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | Das Wörterbuch. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Löscht alle indizierten Daten aus allen Shards des Suchnetzwerks.


