---
title: "WordPattern"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett ordmönster att använda i ordjokerteckensökning."
type: docs
weight: 34
url: /sv/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Representerar ett ordmönster att använda i ordjokerteckensökning.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | Initierar en ny instans av klassen  WordPattern  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Lägger till en sträng i ordmönstret. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Lägger till ett tecken i ordmönstret. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Lägger till en teckenjoker för ett tecken i ordmönstret. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Lägger till en joker för noll eller ett tecken i ordmönstret. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Lägger till en joker för noll eller flera tecken i ordmönstret. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Lägger till en joker för ett eller flera tecken i ordmönstret. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Lägger till en joker i ordmönstret. |
|
|  | [toString()](#toString--) | Returnerar en  System.String  som representerar det aktuella  WordPattern . |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Initierar en ny instans av klassen  WordPattern  .


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Lägger till en sträng i ordmönstret.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | text | java.lang.String | Strängen att lägga till. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Lägger till ett tecken i ordmönstret.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | tecken | char | Tecknet att lägga till. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Lägger till en teckenjoker för ett tecken i ordmönstret.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Lägger till en joker för noll eller ett tecken i ordmönstret.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Lägger till en joker för noll eller flera tecken i ordmönstret.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Lägger till en joker för ett eller flera tecken i ordmönstret.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Lägger till en joker i ordmönstret.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | min | int | Det minsta antalet tecken. |
|
|  | max | int | Det största antalet tecken. |
|

### toString() {#toString--}
```
public String toString()
```


Returnerar en  System.String  som representerar det aktuella  WordPattern .


**Returns:**
java.lang.String - En  System.String  som representerar det aktuella  WordPattern .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
