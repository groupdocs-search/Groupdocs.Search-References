---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Définit l'interface d'un dictionnaire de remplacement de caractères utilisé pendant le processus d'indexation."
type: docs
weight: 16
url: /fr/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Définit l'interface d'un dictionnaire de remplacement de caractères utilisé pendant le processus d'indexation. Le remplacement de caractères peut être utilisé, par exemple, pour supprimer les accents des caractères accentués ou pour créer un index insensible à la casse.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCount()](#getCount--) | Obtient le nombre de caractères contenus dans ce  CharacterReplacementDictionary . |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Ajoute la collection spécifiée de remplacements de caractères à cette instance du  CharacterReplacementDictionary . |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Ajoute la collection spécifiée de remplacements de caractères à cette instance du  CharacterReplacementDictionary . |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Supprime la collection spécifiée de remplacements de caractères de cette instance du  CharacterReplacementDictionary . |
|
|  | [contains(char character)](#contains-char-) | Détermine si un objet  CharacterReplacementDictionary  contient un remplacement pour le caractère spécifié. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Obtient un remplacement pour le caractère spécifié. |
|
|  | [clear()](#clear--) | Supprime tous les remplacements de caractères d'un objet  CharacterReplacementDictionary . |
|
|  | [iterator()](#iterator--) | Retourne un itérateur qui parcourt la collection. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtient le nombre de caractères contenus dans ce  CharacterReplacementDictionary .


**Returns:**
int - Le nombre de caractères dans le dictionnaire.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Ajoute la collection spécifiée de remplacements de caractères à cette instance du  CharacterReplacementDictionary .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | La collection de remplacements de caractères à ajouter au dictionnaire. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Ajoute la collection spécifiée de remplacements de caractères à cette instance du  CharacterReplacementDictionary .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | La collection de remplacements de caractères à ajouter au dictionnaire. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Supprime la collection spécifiée de remplacements de caractères de cette instance du  CharacterReplacementDictionary .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | caractères | char[] | La collection de caractères à supprimer. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Détermine si un objet  CharacterReplacementDictionary  contient un remplacement pour le caractère spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | caractère | char | Le caractère à localiser dans l'objet  CharacterReplacementDictionary . |
|

**Returns:**
booléen -  true  si l'objet  CharacterReplacementDictionary  contient le caractère spécifié ; sinon,  false .

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Obtient un remplacement pour le caractère spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | caractère | char | Le caractère pour lequel obtenir un remplacement. |
|

**Returns:**
char - Le remplacement du caractère spécifié.

### clear() {#clear--}
```
public abstract void clear()
```


Supprime tous les remplacements de caractères d'un objet  CharacterReplacementDictionary .


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Retourne un itérateur qui parcourt la collection.


**Returns:**
java.util.Iterator<java.lang.Character> - Un itérateur qui peut être utilisé pour parcourir la collection.

