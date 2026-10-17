---
title: "SpellingCorrector"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Définit l'interface d'un correcteur orthographique pour les termes d'une requête."
type: docs
weight: 21
url: /fr/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Définit l'interface d'un correcteur orthographique pour les termes d'une requête.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCount()](#getCount--) | Obtient le nombre de mots contenus dans ce  SpellingCorrector . |
|
|  | [getWords()](#getWords--) | Obtient la collection de mots qui est actuellement contenue dans ce  SpellingCorrector . |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Ajoute la collection spécifiée de mots à cette instance du SpellingCorrector. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Ajoute la collection spécifiée de mots à cette instance du SpellingCorrector. |
|
|  | [clear()](#clear--) | Supprime tous les mots d'un objet SpellingCorrector. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtient le nombre de mots contenus dans ce  SpellingCorrector .


**Returns:**
int - Le nombre de mots contenus dans ce SpellingCorrector.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Obtient la collection de mots qui est actuellement contenue dans ce  SpellingCorrector .


**Returns:**
java.lang.String[] - La collection de mots.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Ajoute la collection spécifiée de mots à cette instance du SpellingCorrector.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mots | java.lang.Iterable<java.lang.String> | La collection de mots à ajouter au dictionnaire. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Ajoute la collection spécifiée de mots à cette instance du SpellingCorrector.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mots | java.lang.String[] | La collection de mots à ajouter au dictionnaire. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Supprime tous les mots d'un objet SpellingCorrector.


