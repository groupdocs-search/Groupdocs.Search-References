---
title: "WordPattern"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un modello di parola da utilizzare nella ricerca wildcard di parole."
type: docs
weight: 34
url: /it/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Rappresenta un modello di parola da utilizzare nella ricerca wildcard di parole.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | Inizializza una nuova istanza della classe  WordPattern . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Aggiunge una stringa al modello di parole. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Aggiunge un carattere al modello di parole. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Aggiunge un jolly di un carattere al modello di parole. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Aggiunge un jolly di zero o uno carattere al modello di parole. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Aggiunge un jolly di zero o più caratteri al modello di parole. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Aggiunge un jolly di uno o più caratteri al modello di parole. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Aggiunge un jolly al modello di parole. |
|
|  | [toString()](#toString--) | Restituisce una  System.String  che rappresenta l'attuale  WordPattern . |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Inizializza una nuova istanza della classe  WordPattern .


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Aggiunge una stringa al modello di parole.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | testo | java.lang.String | La stringa da aggiungere. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Aggiunge un carattere al modello di parole.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | carattere | char | Il carattere da aggiungere. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Aggiunge un jolly di un carattere al modello di parole.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Aggiunge un jolly di zero o uno carattere al modello di parole.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Aggiunge un jolly di zero o più caratteri al modello di parole.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Aggiunge un jolly di uno o più caratteri al modello di parole.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Aggiunge un jolly al modello di parole.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | min | int | Il numero minimo di caratteri. |
|
|  | max | int | Il numero massimo di caratteri. |
|

### toString() {#toString--}
```
public String toString()
```


Restituisce una  System.String  che rappresenta l'attuale  WordPattern .


**Returns:**
java.lang.String - Una  System.String  che rappresenta l'attuale  WordPattern .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
