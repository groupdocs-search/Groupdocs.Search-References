---
title: SynonymDictionary
second_title: GroupDocs.Search for Java API Reference
description: Represents a dictionary of synonyms.
type: docs
weight: 22
url: /java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SynonymDictionary extends DictionaryBase implements Iterable<String>
```

Represents a dictionary of synonyms.

**Learn more**

 *  [Synonym search][]
 *  [Managing synonym dictionary][]


[Synonym search]: https://docs.groupdocs.com/display/searchjava/Synonym+search
[Managing synonym dictionary]: https://docs.groupdocs.com/display/searchjava/Synonym+dictionary
## Methods

| Method | Description |
| --- | --- |
| [getCount()](#getCount--) | Gets the number of words contained in this  SynonymDictionary . |
| [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Adds the specified collection of synonym groups to this instance of the  SynonymDictionary . |
| [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Adds the specified collection of synonym groups to this instance of the  SynonymDictionary . |
| [clear()](#clear--) | Removes all words from this  SynonymDictionary  object. |
| [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Gets the synonyms for the specified word. |
| [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Gets all groups of synonyms to which the specified word belongs. |
| [getAllSynonymGroups()](#getAllSynonymGroups--) | Gets all groups of synonyms contained in this dictionary. |
| [iterator()](#iterator--) | Returns an iterator that iterates through the collection. |
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gets the number of words contained in this  SynonymDictionary .

**Returns:**
int - The number of words contained in this  SynonymDictionary .
### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Adds the specified collection of synonym groups to this instance of the  SynonymDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| synonyms | java.lang.Iterable<java.lang.String[]> | The collection of synonym groups to add to the dictionary. |

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Adds the specified collection of synonym groups to this instance of the  SynonymDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| synonyms | java.lang.String[][] | The collection of synonym groups to add to the dictionary. |

### clear() {#clear--}
```
public abstract void clear()
```


Removes all words from this  SynonymDictionary  object.

### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Gets the synonyms for the specified word. The resulting array does not contain the original word.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| word | java.lang.String | The word to suggest the synonyms. |

**Returns:**
java.lang.String[] - The synonyms for the specified word or empty array if the  SynonymDictionary  object does not contain the specified word.
### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Gets all groups of synonyms to which the specified word belongs.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| word | java.lang.String | The word for getting groups of synonyms. |

**Returns:**
java.lang.String[][] - All groups of synonyms to which the specified word belongs.
### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Gets all groups of synonyms contained in this dictionary.

**Returns:**
java.lang.String[][] - All groups of synonyms.
### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returns an iterator that iterates through the collection.

**Returns:**
java.util.Iterator<java.lang.String> - An iterator that can be used to iterate through the collection.
