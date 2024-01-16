---
title: CharacterReplacementDictionary
second_title: GroupDocs.Search for Java API Reference
description: Defines interface of a character replacement dictionary that is used during the indexing process.
type: docs
weight: 16
url: /java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Defines interface of a character replacement dictionary that is used during the indexing process. Character replacement can be used, for example, to remove accents from accented characters or to make case-insensitive index.

**Learn more**

 *  [Character replacement during Indexing][]
 *  [Managing character replacements][]


[Character replacement during Indexing]: https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing
[Managing character replacements]: https://docs.groupdocs.com/display/searchjava/Character+replacements
## Methods

| Method | Description |
| --- | --- |
| [getCount()](#getCount--) | Gets the number of characters contained in this  CharacterReplacementDictionary . |
| [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Adds the specified collection of character replacements to this instance of the  CharacterReplacementDictionary . |
| [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Adds the specified collection of character replacements to this instance of the  CharacterReplacementDictionary . |
| [removeRange(char[] characters)](#removeRange-char---) | Removes the specified collection of character replacements from this instance of the  CharacterReplacementDictionary . |
| [contains(char character)](#contains-char-) | Determines whether a  CharacterReplacementDictionary  object contains a replacement for the specified character. |
| [getReplacement(char character)](#getReplacement-char-) | Gets a replacement for the specified character. |
| [clear()](#clear--) | Removes all character replacements from a  CharacterReplacementDictionary  object. |
| [iterator()](#iterator--) | Returns an iterator that iterates through the collection. |
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gets the number of characters contained in this  CharacterReplacementDictionary .

**Returns:**
int - The number of characters in the dictionary.
### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Adds the specified collection of character replacements to this instance of the  CharacterReplacementDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | The collection of character replacements to add to the dictionary. |

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Adds the specified collection of character replacements to this instance of the  CharacterReplacementDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | The collection of character replacements to add to the dictionary. |

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Removes the specified collection of character replacements from this instance of the  CharacterReplacementDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| characters | char[] | The collection of characters to remove. |

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Determines whether a  CharacterReplacementDictionary  object contains a replacement for the specified character.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| character | char | The character to locate in the  CharacterReplacementDictionary  object. |

**Returns:**
boolean -  true  if the  CharacterReplacementDictionary  object contains the specified character; otherwise,  false .
### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Gets a replacement for the specified character.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| character | char | The character to get a replacement for. |

**Returns:**
char - The replacement for the specified character.
### clear() {#clear--}
```
public abstract void clear()
```


Removes all character replacements from a  CharacterReplacementDictionary  object.

### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Returns an iterator that iterates through the collection.

**Returns:**
java.util.Iterator<java.lang.Character> - An iterator that can be used to iterate through the collection.
