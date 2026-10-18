---
title: "Alfabet"
second_title: "GroupDocs.Search för Java API-referens"
description: "Definierar gränssnittet för en teckenordbok som används under indexering för att upptäcka teckentyp."
type: docs
weight: 15
url: /sv/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Definierar gränssnittet för en teckendiktionär som används under indexering för att upptäcka teckentyp. Varje tecken kan hanteras som separator, som bokstav eller båda.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Hämtar en typ av ett tecken. |
|
|  | [getCount()](#getCount--) | Hämtar antalet tecken som finns i  Alphabet . |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Ställer in typen för varje tecken i den angivna samlingen i denna instans av  Alphabet . |
|
|  | [clear()](#clear--) | Ställer in  CharacterType.Separator  typen för alla tecken i detta  Alphabet . |
|
|  | [iterator()](#iterator--) | Returnerar en iterator som itererar genom samlingen. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Hämtar en typ av ett tecken.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tecken | char | Tecknet för att få en typ. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet tecken som finns i  Alphabet .


**Returns:**
int - Antalet tecken i ordboken.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Ställer in typen för varje tecken i den angivna samlingen i denna instans av  Alphabet .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tecken | char[] | Samlingen av tecken för att ställa in typen. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | Teckentypen. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Ställer in  CharacterType.Separator  typen för alla tecken i detta  Alphabet .


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Returnerar en iterator som itererar genom samlingen.


**Returns:**
java.util.Iterator<java.lang.Character> - En iterator som kan användas för att iterera genom samlingen.

