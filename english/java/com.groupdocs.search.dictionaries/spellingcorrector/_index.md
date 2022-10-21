---
title: SpellingCorrector
second_title: GroupDocs.Search for Java API Reference
description: Represents a spelling corrector for terms in a query.
type: docs
weight: 20
url: /java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public abstract class SpellingCorrector extends DictionaryBase
```

Represents a spelling corrector for terms in a query.

**Learn more**

 *  [Spell checking][]
 *  [Managing spelling corrector][]


[Spell checking]: https://docs.groupdocs.com/display/searchjava/Spell+checking
[Managing spelling corrector]: https://docs.groupdocs.com/display/searchjava/Spelling+corrector
## Methods

| Method | Description |
| --- | --- |
| [getCount()](#getCount--) | Gets the number of words contained in this  SpellingCorrector . |
| [getWords()](#getWords--) | Gets the collection of words that is currently contained in this  SpellingCorrector . |
| [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Adds the specified collection of words to this instance of the  SpellingCorrector . |
| [addRange(String[] words)](#addRange-java.lang.String---) | Adds the specified collection of words to this instance of the  SpellingCorrector . |
| [clear()](#clear--) | Removes all words from a  SpellingCorrector  object. |
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gets the number of words contained in this  SpellingCorrector .

**Returns:**
int - The number of words contained in this  SpellingCorrector .
### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Gets the collection of words that is currently contained in this  SpellingCorrector .

**Returns:**
java.lang.String[] - The collection of words.
### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Adds the specified collection of words to this instance of the  SpellingCorrector .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| words | java.lang.Iterable<java.lang.String> | The collection of words to add to the dictionary. |

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Adds the specified collection of words to this instance of the  SpellingCorrector .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| words | java.lang.String[] | The collection of words to add to the dictionary. |

### clear() {#clear--}
```
public abstract void clear()
```


Removes all words from a  SpellingCorrector  object.

