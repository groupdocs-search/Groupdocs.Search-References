---
title: "WordPattern"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een woordpatroon voor om te gebruiken in woordjokerteken-zoekopdrachten."
type: docs
weight: 34
url: /nl/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Stelt een woordpatroon voor om te gebruiken in woordjokerteken-zoekopdrachten.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | Initialiseert een nieuw exemplaar van de  WordPattern  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Voegt een tekenreeks toe aan het woordpatroon. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Voegt een teken toe aan het woordpatroon. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Voegt een één-teken wildcard toe aan het woordpatroon. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Voegt een nul-of-één-teken wildcard toe aan het woordpatroon. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Voegt een nul-of-meerdere-tekens wildcard toe aan het woordpatroon. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Voegt een één-of-meerdere-tekens wildcard toe aan het woordpatroon. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Voegt een wildcard toe aan het woordpatroon. |
|
|  | [toString()](#toString--) | Retourneert een  System.String  die de huidige  WordPattern  weergeeft. |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Initialiseert een nieuw exemplaar van de  WordPattern  klasse.


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Voegt een tekenreeks toe aan het woordpatroon.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tekst | java.lang.String | De string om toe te voegen. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Voegt een teken toe aan het woordpatroon.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | teken | char | Het teken om toe te voegen. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Voegt een één-teken wildcard toe aan het woordpatroon.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Voegt een nul-of-één-teken wildcard toe aan het woordpatroon.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Voegt een nul-of-meerdere-tekens wildcard toe aan het woordpatroon.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Voegt een één-of-meerdere-tekens wildcard toe aan het woordpatroon.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Voegt een wildcard toe aan het woordpatroon.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | min | int | Het minimum aantal tekens. |
|
|  | max | int | Het maximum aantal tekens. |
|

### toString() {#toString--}
```
public String toString()
```


Retourneert een  System.String  die de huidige  WordPattern  weergeeft.


**Returns:**
java.lang.String - Een  System.String  die de huidige  WordPattern  weergeeft.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
