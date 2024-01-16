---
title: StopWordDictionary
second_title: GroupDocs.Search for Java API Reference
description: Defines interface of a dictionary of stop words.
type: docs
weight: 22
url: /java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Defines interface of a dictionary of stop words.

**Learn more**

 *  [Indexing with stop words][]
 *  [Managing stop word dictionary][]


[Indexing with stop words]: https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words
[Managing stop word dictionary]: https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary
## Methods

| Method | Description |
| --- | --- |
| [getCount()](#getCount--) | Gets the number of stop words contained in the  StopWordDictionary . |
| [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Adds the specified collection of words to this instance of the  StopWordDictionary . |
| [addRange(String[] words)](#addRange-java.lang.String---) | Adds the specified collection of words to this instance of the  StopWordDictionary . |
| [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Removes the specified collection of words from this instance of the  StopWordDictionary . |
| [removeRange(String[] words)](#removeRange-java.lang.String---) | Removes the specified collection of words from this instance of the  StopWordDictionary . |
| [contains(String word)](#contains-java.lang.String-) | Determines whether a  StopWordDictionary  object contains the specified word. |
| [clear()](#clear--) | Removes all words from a  StopWordDictionary  object. |
| [iterator()](#iterator--) | Returns an iterator that iterates through the collection. |
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gets the number of stop words contained in the  StopWordDictionary .

**Returns:**
int - The number of stop words in the dictionary.
### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Adds the specified collection of words to this instance of the  StopWordDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| words | java.lang.Iterable<java.lang.String> | The collection of words to add to the dictionary. |

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Adds the specified collection of words to this instance of the  StopWordDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| words | java.lang.String[] | The collection of words to add to the dictionary. |

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Removes the specified collection of words from this instance of the  StopWordDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| words | java.lang.Iterable<java.lang.String> | The collection of words to remove. |

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Removes the specified collection of words from this instance of the  StopWordDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| words | java.lang.String[] | The collection of words to remove. |

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Determines whether a  StopWordDictionary  object contains the specified word.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| word | java.lang.String | The word to locate in the  StopWordDictionary  object. |

**Returns:**
boolean -  true  if the  StopWordDictionary  object contains the specified word; otherwise,  false .
### clear() {#clear--}
```
public abstract void clear()
```


Removes all words from a  StopWordDictionary  object.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returns an iterator that iterates through the collection.

**Returns:**
java.util.Iterator<java.lang.String> - An iterator that can be used to iterate through the collection.
