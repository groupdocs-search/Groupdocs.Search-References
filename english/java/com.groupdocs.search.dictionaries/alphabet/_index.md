---
title: Alphabet
second_title: GroupDocs.Search for Java API Reference
description: Defines interface of a dictionary of characters that is used during indexing to detect character type.
type: docs
weight: 15
url: /java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Defines interface of a dictionary of characters that is used during indexing to detect character type. Each character can be handled as separator, as letter, or both.

**Learn more**

 *  [Character types][]
 *  [Managing alphabet][]


[Character types]: https://docs.groupdocs.com/display/searchjava/Character+types
[Managing alphabet]: https://docs.groupdocs.com/display/searchjava/Alphabet
## Methods

| Method | Description |
| --- | --- |
| [getCharacterType(char character)](#getCharacterType-char-) | Gets a type of a character. |
| [getCount()](#getCount--) | Gets the number of characters contained in the  Alphabet . |
| [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Sets the type for each character of the specified collection in this instance of the  Alphabet . |
| [clear()](#clear--) | Sets the  CharacterType.Separator  type for all characters in this  Alphabet . |
| [iterator()](#iterator--) | Returns an iterator that iterates through the collection. |
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Gets a type of a character.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| character | char | The character to get a type. |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gets the number of characters contained in the  Alphabet .

**Returns:**
int - The number of characters in the dictionary.
### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Sets the type for each character of the specified collection in this instance of the  Alphabet .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| characters | char[] | The collection of characters to set the type. |
| type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | The character type. |

### clear() {#clear--}
```
public abstract void clear()
```


Sets the  CharacterType.Separator  type for all characters in this  Alphabet .

### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Returns an iterator that iterates through the collection.

**Returns:**
java.util.Iterator<java.lang.Character> - An iterator that can be used to iterate through the collection.
