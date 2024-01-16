---
title: Indexer
second_title: GroupDocs.Search for Java API Reference
description: Represents a service that manages the distribution of indexed documents across shards of the search network.
type: docs
weight: 10
url: /java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

Represents a service that manages the distribution of indexed documents across shards of the search network.
## Constructors

| Constructor | Description |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## Methods

| Method | Description |
| --- | --- |
| [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Performs indexing operation. |
| [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | Deletes indexed documents. |
| [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | Minimizes the number of index segments by merging them one with another. |
| [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | Synchronizes the list of indexed documents with those on shards. |
| [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | Applies the specified batch of attribute changes to indexed documents without reindexing. |
| [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | Gets all the attributes associated with the specified indexed document. |
| [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | Gets a dictionary from the specified shard. |
| [getAlphabet(int shardIndex)](#getAlphabet-int-) | Gets the alphabet dictionary. |
| [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | Gets the alias dictionary. |
| [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | Gets the character replacement dictionary. |
| [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | Gets the synonym dictionary. |
| [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | Gets the homophone dictionary. |
| [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | Gets the spelling corrector dictionary. |
| [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | Gets the stop word dictionary. |
| [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | Gets the password dictionary. |
| [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | Sets a dictionary in the specified shard. |
| [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | Sets a dictionary in all shards. |
| [deleteAllData()](#deleteAllData--) | Deletes all indexed data from all shards of the search network. |
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


Performs indexing operation. Indexing only from stream and structure is supported.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documents | [Document\[\]](../../com.groupdocs.search/document) | The documents from file system, stream, or structure. |
| passwords | java.lang.String[] | The document passwords. |
| options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | The add options. |

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


Deletes indexed documents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentKeys | java.lang.String[] | The keys of documents added from streams or structures. |
| options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | The delete options. |

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


Minimizes the number of index segments by merging them one with another. This operation improves search performance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | The optimize options. |

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


Synchronizes the list of indexed documents with those on shards. This operation fixes issues with indexing and deletion of documents that resulted from communication problems with the search network nodes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | The synchronize options. |

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


Applies the specified batch of attribute changes to indexed documents without reindexing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | The attribute change batch. |
| options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | The change attributes options. |

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


Gets all the attributes associated with the specified indexed document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentKey | java.lang.String | The document key. |

**Returns:**
java.lang.String[] - The attributes associated with the specified indexed document.
### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


Gets a dictionary from the specified shard.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | The dictionary type. |
| shardIndex | int | The shard index. |

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.
### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


Gets the alphabet dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shardIndex | int | The shard index. |

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.
### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


Gets the alias dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shardIndex | int | The shard index. |

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.
### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


Gets the character replacement dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shardIndex | int | The shard index. |

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.
### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


Gets the synonym dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shardIndex | int | The shard index. |

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.
### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


Gets the homophone dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shardIndex | int | The shard index. |

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.
### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


Gets the spelling corrector dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shardIndex | int | The shard index. |

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.
### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


Gets the stop word dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shardIndex | int | The shard index. |

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.
### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


Gets the password dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| shardIndex | int | The shard index. |

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.
### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


Sets a dictionary in the specified shard.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | The dictionary. |
| shardIndex | int | The shard index. |

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


Sets a dictionary in all shards.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | The dictionary. |

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


Deletes all indexed data from all shards of the search network.

