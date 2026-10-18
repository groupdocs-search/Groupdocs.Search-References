---
title: "WordPattern"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein Wortmuster dar, das bei der Wort-Platzhaltersuche verwendet wird."
type: docs
weight: 34
url: /de/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Stellt ein Wortmuster dar, das bei der Wort-Platzhaltersuche verwendet wird.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | Initialisiert eine neue Instanz der  WordPattern  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Fügt dem Wortmuster eine Zeichenkette hinzu. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Fügt dem Wortmuster ein Zeichen hinzu. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Fügt dem Wortmuster einen einzeichenigen Platzhalter hinzu. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Fügt dem Wortmuster einen Platzhalter für null oder ein Zeichen hinzu. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Fügt dem Wortmuster einen Platzhalter für null oder mehrere Zeichen hinzu. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Fügt dem Wortmuster einen Platzhalter für ein oder mehrere Zeichen hinzu. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Fügt dem Wortmuster einen Platzhalter hinzu. |
|
|  | [toString()](#toString--) | Gibt einen  System.String  zurück, der das aktuelle  WordPattern  darstellt. |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Initialisiert eine neue Instanz der  WordPattern  Klasse.


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Fügt dem Wortmuster eine Zeichenkette hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Text | java.lang.String | Die Zeichenkette zum Anhängen. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Fügt dem Wortmuster ein Zeichen hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Zeichen | char | Das Zeichen zum Anhängen. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Fügt dem Wortmuster einen einzeichenigen Platzhalter hinzu.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Fügt dem Wortmuster einen Platzhalter für null oder ein Zeichen hinzu.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Fügt dem Wortmuster einen Platzhalter für null oder mehrere Zeichen hinzu.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Fügt dem Wortmuster einen Platzhalter für ein oder mehrere Zeichen hinzu.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Fügt dem Wortmuster einen Platzhalter hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | min | int | Die minimale Anzahl von Zeichen. |
|
|  | max | int | Die maximale Anzahl von Zeichen. |
|

### toString() {#toString--}
```
public String toString()
```


Gibt einen  System.String  zurück, der das aktuelle  WordPattern  darstellt.


**Returns:**
java.lang.String - Ein  System.String  der das aktuelle  WordPattern  darstellt.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
