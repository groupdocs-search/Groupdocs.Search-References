---
title: "Alphabet"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Définit l'interface d'un dictionnaire de caractères utilisé lors de l'indexation pour détecter le type de caractère."
type: docs
weight: 15
url: /fr/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Définit l'interface d'un dictionnaire de caractères utilisé lors de l'indexation pour détecter le type de caractère. Chaque caractère peut être traité comme séparateur, comme lettre, ou les deux.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Obtient le type d'un caractère. |
|
|  | [getCount()](#getCount--) | Obtient le nombre de caractères contenus dans l'  Alphabet . |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Définit le type pour chaque caractère de la collection spécifiée dans cette instance de l'  Alphabet . |
|
|  | [clear()](#clear--) | Définit le type  CharacterType.Separator  pour tous les caractères de cet  Alphabet . |
|
|  | [iterator()](#iterator--) | Retourne un itérateur qui parcourt la collection. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Obtient le type d'un caractère.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | caractère | char | Le caractère pour obtenir un type. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtient le nombre de caractères contenus dans l'  Alphabet .


**Returns:**
int - Le nombre de caractères dans le dictionnaire.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Définit le type pour chaque caractère de la collection spécifiée dans cette instance de l'  Alphabet .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | caractères | char[] | La collection de caractères pour définir le type. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | Le type de caractère. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Définit le type  CharacterType.Separator  pour tous les caractères de cet  Alphabet .


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Retourne un itérateur qui parcourt la collection.


**Returns:**
java.util.Iterator<java.lang.Character> - Un itérateur qui peut être utilisé pour parcourir la collection.

