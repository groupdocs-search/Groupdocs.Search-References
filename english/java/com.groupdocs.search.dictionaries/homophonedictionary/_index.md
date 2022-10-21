---
title: HomophoneDictionary
second_title: GroupDocs.Search for Java API Reference
description: Represents a dictionary of heterographic homophones.
type: docs
weight: 18
url: /java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class HomophoneDictionary extends DictionaryBase implements Iterable<String>
```

Represents a dictionary of heterographic homophones.

**Learn more**

 *  [Homophone search][]
 *  [Managing homophone dictionary][]


[Homophone search]: https://docs.groupdocs.com/display/searchjava/Homophone+search
[Managing homophone dictionary]: https://docs.groupdocs.com/display/searchjava/Homophone+dictionary
## Methods

| Method | Description |
| --- | --- |
| [getCount()](#getCount--) | Gets the number of words contained in this  HomophoneDictionary . |
| [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Adds the specified collection of homophone groups to this instance of the  HomophoneDictionary . |
| [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Adds the specified collection of homophone groups to this instance of the  HomophoneDictionary . |
| [clear()](#clear--) | Removes all words from a  HomophoneDictionary  object. |
| [getHomophones(String word)](#getHomophones-java.lang.String-) | Gets the homophones for the specified word. |
| [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Gets all groups of homophones to which the specified word belongs. |
| [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Gets all groups of homophones contained in this dictionary. |
| [iterator()](#iterator--) | Returns an iterator that iterates through the collection. |
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gets the number of words contained in this  HomophoneDictionary .

**Returns:**
int - The number of words.
### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Adds the specified collection of homophone groups to this instance of the  HomophoneDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| homophones | java.lang.Iterable<java.lang.String[]> | The collection of homophone groups to add to the dictionary. |

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Adds the specified collection of homophone groups to this instance of the  HomophoneDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| homophones | java.lang.String[][] | The collection of homophone groups to add to the dictionary. |

### clear() {#clear--}
```
public abstract void clear()
```


Removes all words from a  HomophoneDictionary  object.

### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Gets the homophones for the specified word. The resulting array does not contain the original word.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| word | java.lang.String | The word to suggest the homophones. |

**Returns:**
java.lang.String[] - The homophones for the specified word or empty array if the  HomophoneDictionary  object does not contain the specified word.
### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Gets all groups of homophones to which the specified word belongs.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| word | java.lang.String | The word for getting groups of homophones. |

**Returns:**
java.lang.String[][] - All groups of homophones to which the specified word belongs.
### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Gets all groups of homophones contained in this dictionary.

**Returns:**
java.lang.String[][] - All groups of homophones.
### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returns an iterator that iterates through the collection.

**Returns:**
java.util.Iterator<java.lang.String> - An iterator that can be used to iterate through the collection.
