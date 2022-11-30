---
title: WordPattern
second_title: GroupDocs.Search for Java API Reference
description: Represents a word pattern to use in word wildcard search.
type: docs
weight: 36
url: /java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Represents a word pattern to use in word wildcard search.

**Learn more**

 *  [Wildcard search][]
 *  [Phrase search][]


[Wildcard search]: https://docs.groupdocs.com/display/searchjava/Wildcard+search
[Phrase search]: https://docs.groupdocs.com/display/searchjava/Phrase+search
## Constructors

| Constructor | Description |
| --- | --- |
| [WordPattern()](#WordPattern--) | Initializes a new instance of the  WordPattern  class. |
## Methods

| Method | Description |
| --- | --- |
| [appendString(String text)](#appendString-java.lang.String-) | Appends a string to the word pattern. |
| [appendCharacter(char character)](#appendCharacter-char-) | Appends a character to the word pattern. |
| [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Appends one character wildcard to the word pattern. |
| [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Appends zero or one character wildcard to the word pattern. |
| [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Appends zero or more characters wildcard to the word pattern. |
| [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Appends one or more characters wildcard to the word pattern. |
| [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Appends a wildcard to the word pattern. |
| [toString()](#toString--) | Returns a  System.String  that represents the current  WordPattern . |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Initializes a new instance of the  WordPattern  class.

### appendString(String text) {#appendString-java.lang.String-}
```
public final void appendString(String text)
```


Appends a string to the word pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The string to append. |

### appendCharacter(char character) {#appendCharacter-char-}
```
public final void appendCharacter(char character)
```


Appends a character to the word pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| character | char | The character to append. |

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public final void appendOneCharacterWildcard()
```


Appends one character wildcard to the word pattern.

### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public final void appendZeroOrOneCharacterWildcard()
```


Appends zero or one character wildcard to the word pattern.

### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public final void appendZeroOrMoreCharactersWildcard()
```


Appends zero or more characters wildcard to the word pattern.

### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public final void appendOneOrMoreCharactersWildcard()
```


Appends one or more characters wildcard to the word pattern.

### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public final void appendWildcard(int min, int max)
```


Appends a wildcard to the word pattern.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| min | int | The minimum number of characters. |
| max | int | The maximum number of characters. |

### toString() {#toString--}
```
public String toString()
```


Returns a  System.String  that represents the current  WordPattern .

**Returns:**
java.lang.String - A  System.String  that represents the current  WordPattern .
