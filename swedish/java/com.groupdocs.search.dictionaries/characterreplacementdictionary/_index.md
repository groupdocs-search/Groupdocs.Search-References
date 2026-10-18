---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search för Java API-referens"
description: "Definierar gränssnittet för en teckenersättningsordbok som används under indexeringsprocessen."
type: docs
weight: 16
url: /sv/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Definierar gränssnittet för en teckenersättningsordbok som används under indexeringsprocessen. Teckenersättning kan exempelvis användas för att ta bort accenter från accentuerade tecken eller för att skapa ett skiftlägesokänsligt index.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCount()](#getCount--) | Hämtar antalet tecken som finns i denna  CharacterReplacementDictionary . |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Lägger till den angivna samlingen av teckenersättningar till denna instans av  CharacterReplacementDictionary . |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Lägger till den angivna samlingen av teckenersättningar till denna instans av  CharacterReplacementDictionary . |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Tar bort den angivna samlingen av teckenersättningar från denna instans av  CharacterReplacementDictionary . |
|
|  | [contains(char character)](#contains-char-) | Avgör om ett  CharacterReplacementDictionary  -objekt innehåller en ersättning för det angivna tecknet. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Hämtar en ersättning för det angivna tecknet. |
|
|  | [clear()](#clear--) | Tar bort alla teckenersättningar från ett  CharacterReplacementDictionary  -objekt. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator som itererar genom samlingen. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet tecken som finns i denna  CharacterReplacementDictionary .


**Returns:**
int - Antalet tecken i ordboken.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Lägger till den angivna samlingen av teckenersättningar till denna instans av  CharacterReplacementDictionary .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | Samlingen av teckenersättningar att lägga till i ordboken. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Lägger till den angivna samlingen av teckenersättningar till denna instans av  CharacterReplacementDictionary .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | Samlingen av teckenersättningar att lägga till i ordboken. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Tar bort den angivna samlingen av teckenersättningar från denna instans av  CharacterReplacementDictionary .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tecken | char[] | Samlingen av tecken att ta bort. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Avgör om ett  CharacterReplacementDictionary  -objekt innehåller en ersättning för det angivna tecknet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tecken | char | Tecknet att leta upp i  CharacterReplacementDictionary  -objektet. |
|

**Returns:**
boolean -  true  om  CharacterReplacementDictionary  -objektet innehåller det angivna tecknet; annars  false .

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Hämtar en ersättning för det angivna tecknet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tecken | char | Tecknet att hämta en ersättning för. |
|

**Returns:**
char - Ersättningen för det angivna tecknet.

### clear() {#clear--}
```
public abstract void clear()
```


Tar bort alla teckenersättningar från ett  CharacterReplacementDictionary  -objekt.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Returnerar en iterator som itererar genom samlingen.


**Returns:**
java.util.Iterator<java.lang.Character> - En iterator som kan användas för att iterera genom samlingen.

