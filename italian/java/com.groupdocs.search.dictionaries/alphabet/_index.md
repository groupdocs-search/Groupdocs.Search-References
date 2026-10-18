---
title: "Alfabeto"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Definisce l'interfaccia di un dizionario di caratteri utilizzato durante l'indicizzazione per rilevare il tipo di carattere."
type: docs
weight: 15
url: /it/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Definisce l'interfaccia di un dizionario di caratteri che viene usato durante l'indicizzazione per rilevare il tipo di carattere. Ogni carattere può essere gestito come separatore, come lettera, o entrambi.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Ottiene un tipo di carattere. |
|
|  | [getCount()](#getCount--) | Ottiene il numero di caratteri contenuti nell'  Alphabet . |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Imposta il tipo per ogni carattere della collezione specificata in questa istanza dell'  Alphabet . |
|
|  | [clear()](#clear--) | Imposta il tipo  CharacterType.Separator  per tutti i caratteri in questo  Alphabet . |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore che scorre la collezione. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Ottiene un tipo di carattere.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | carattere | char | Il carattere per ottenere un tipo. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Ottiene il numero di caratteri contenuti nell'  Alphabet .


**Returns:**
int - Il numero di caratteri nel dizionario.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Imposta il tipo per ogni carattere della collezione specificata in questa istanza dell'  Alphabet .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | caratteri | char[] | La collezione di caratteri per impostare il tipo. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | Il tipo di carattere. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Imposta il tipo  CharacterType.Separator  per tutti i caratteri in questo  Alphabet .


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Restituisce un iteratore che scorre la collezione.


**Returns:**
java.util.Iterator<java.lang.Character> - Un iteratore che può essere usato per iterare attraverso la collezione.

