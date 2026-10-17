---
title: "WordPattern"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un modèle de mot à utiliser dans la recherche de mots avec caractères génériques."
type: docs
weight: 34
url: /fr/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Représente un modèle de mot à utiliser dans la recherche de mots avec caractères génériques.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | Initialise une nouvelle instance de la classe  WordPattern . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Ajoute une chaîne au modèle de mot. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Ajoute un caractère au modèle de mot. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Ajoute un joker d'un caractère au modèle de mot. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Ajoute un joker de zéro ou un caractère au modèle de mot. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Ajoute un joker de zéro ou plusieurs caractères au modèle de mot. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Ajoute un joker d'un ou plusieurs caractères au modèle de mot. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Ajoute un joker au modèle de mot. |
|
|  | [toString()](#toString--) | Renvoie une  System.String  qui représente le  WordPattern  actuel. |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Initialise une nouvelle instance de la classe  WordPattern .


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Ajoute une chaîne au modèle de mot.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | texte | java.lang.String | La chaîne à ajouter. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Ajoute un caractère au modèle de mot.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | caractère | char | Le caractère à ajouter. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Ajoute un joker d'un caractère au modèle de mot.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Ajoute un joker de zéro ou un caractère au modèle de mot.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Ajoute un joker de zéro ou plusieurs caractères au modèle de mot.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Ajoute un joker d'un ou plusieurs caractères au modèle de mot.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Ajoute un joker au modèle de mot.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | min | int | Le nombre minimum de caractères. |
|
|  | max | int | Le nombre maximum de caractères. |
|

### toString() {#toString--}
```
public String toString()
```


Renvoie une  System.String  qui représente le  WordPattern  actuel.


**Returns:**
java.lang.String - Une  System.String  qui représente le  WordPattern  actuel.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
