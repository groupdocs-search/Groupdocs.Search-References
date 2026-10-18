---
title: "Alfabeto"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Define la interfaz de un diccionario de caracteres que se utiliza durante la indexación para detectar el tipo de carácter."
type: docs
weight: 15
url: /es/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Define la interfaz de un diccionario de caracteres que se utiliza durante la indexación para detectar el tipo de carácter. Cada carácter puede manejarse como separador, como letra o como ambos.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Obtiene un tipo de carácter. |
|
|  | [getCount()](#getCount--) | Obtiene el número de caracteres contenidos en el Alfabeto. |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Establece el tipo para cada carácter de la colección especificada en esta instancia del Alfabeto. |
|
|  | [clear()](#clear--) | Establece el tipo CharacterType.Separator para todos los caracteres en este Alfabeto. |
|
|  | [iterator()](#iterator--) | Devuelve un iterador que recorre la colección. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Obtiene un tipo de carácter.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | carácter | char | El carácter para obtener un tipo. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el número de caracteres contenidos en el Alfabeto.


**Returns:**
int - El número de caracteres en el diccionario.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Establece el tipo para cada carácter de la colección especificada en esta instancia del Alfabeto.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | caracteres | char[] | La colección de caracteres para establecer el tipo. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | El tipo de carácter. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Establece el tipo CharacterType.Separator para todos los caracteres en este Alfabeto.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Devuelve un iterador que recorre la colección.


**Returns:**
java.util.Iterator<java.lang.Character> - Un iterador que puede usarse para iterar a través de la colección.

