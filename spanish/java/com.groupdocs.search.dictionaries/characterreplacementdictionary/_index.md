---
title: "CharacterReplacementDictionary"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Define la interfaz de un diccionario de reemplazo de caracteres que se utiliza durante el proceso de indexación."
type: docs
weight: 16
url: /es/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Define la interfaz de un diccionario de reemplazo de caracteres que se utiliza durante el proceso de indexación. El reemplazo de caracteres puede usarse, por ejemplo, para eliminar acentos de caracteres acentuados o para crear un índice que no distinga entre mayúsculas y minúsculas.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCount()](#getCount--) | Obtiene el número de caracteres contenidos en este  CharacterReplacementDictionary . |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Agrega la colección especificada de reemplazos de caracteres a esta instancia del  CharacterReplacementDictionary . |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Agrega la colección especificada de reemplazos de caracteres a esta instancia del  CharacterReplacementDictionary . |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Elimina la colección especificada de reemplazos de caracteres de esta instancia del  CharacterReplacementDictionary . |
|
|  | [contains(char character)](#contains-char-) | Determina si un objeto  CharacterReplacementDictionary  contiene un reemplazo para el carácter especificado. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Obtiene un reemplazo para el carácter especificado. |
|
|  | [clear()](#clear--) | Elimina todos los reemplazos de caracteres de un objeto  CharacterReplacementDictionary . |
|
|  | [iterator()](#iterator--) | Devuelve un iterador que recorre la colección. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el número de caracteres contenidos en este  CharacterReplacementDictionary .


**Returns:**
int - El número de caracteres en el diccionario.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Agrega la colección especificada de reemplazos de caracteres a esta instancia del  CharacterReplacementDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | La colección de reemplazos de caracteres que se agregarán al diccionario. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Agrega la colección especificada de reemplazos de caracteres a esta instancia del  CharacterReplacementDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | La colección de reemplazos de caracteres que se agregarán al diccionario. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Elimina la colección especificada de reemplazos de caracteres de esta instancia del  CharacterReplacementDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | caracteres | char[] | La colección de caracteres que se eliminarán. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Determina si un objeto  CharacterReplacementDictionary  contiene un reemplazo para el carácter especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | carácter | char | El carácter a localizar en el objeto  CharacterReplacementDictionary . |
|

**Returns:**
boolean -  true  si el objeto  CharacterReplacementDictionary  contiene el carácter especificado; de lo contrario,  false .

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Obtiene un reemplazo para el carácter especificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | carácter | char | El carácter para el cual obtener un reemplazo. |
|

**Returns:**
char - El reemplazo para el carácter especificado.

### clear() {#clear--}
```
public abstract void clear()
```


Elimina todos los reemplazos de caracteres de un objeto  CharacterReplacementDictionary .


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Devuelve un iterador que recorre la colección.


**Returns:**
java.util.Iterator<java.lang.Character> - Un iterador que puede usarse para iterar a través de la colección.

