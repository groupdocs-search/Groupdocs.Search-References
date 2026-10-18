---
title: "WordPattern"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un patrón de palabra para usar en la búsqueda de comodines de palabras."
type: docs
weight: 34
url: /es/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Representa un patrón de palabra para usar en la búsqueda de comodines de palabras.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | Inicializa una nueva instancia de la clase  WordPattern . |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Agrega una cadena al patrón de palabra. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Agrega un carácter al patrón de palabra. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Agrega un comodín de un carácter al patrón de palabra. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Agrega un comodín de cero o un carácter al patrón de palabra. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Agrega un comodín de cero o más caracteres al patrón de palabra. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Agrega un comodín de uno o más caracteres al patrón de palabra. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Agrega un comodín al patrón de palabra. |
|
|  | [toString()](#toString--) | Devuelve un  System.String  que representa el  WordPattern  actual. |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Inicializa una nueva instancia de la clase  WordPattern .


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Agrega una cadena al patrón de palabra.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | texto | java.lang.String | La cadena a añadir. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Agrega un carácter al patrón de palabra.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | carácter | char | El carácter a añadir. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Agrega un comodín de un carácter al patrón de palabra.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Agrega un comodín de cero o un carácter al patrón de palabra.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Agrega un comodín de cero o más caracteres al patrón de palabra.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Agrega un comodín de uno o más caracteres al patrón de palabra.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Agrega un comodín al patrón de palabra.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | mín | int | El número mínimo de caracteres. |
|
|  | máx | int | El número máximo de caracteres. |
|

### toString() {#toString--}
```
public String toString()
```


Devuelve un  System.String  que representa el  WordPattern  actual.


**Returns:**
java.lang.String - Un  System.String  que representa el  WordPattern  actual.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
