---
title: "StopWordDictionary"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Définit l'interface d'un dictionnaire de mots vides."
type: docs
weight: 22
url: /fr/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Définit l'interface d'un dictionnaire de mots vides.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCount()](#getCount--) | Obtient le nombre de mots vides contenus dans le StopWordDictionary. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Ajoute la collection spécifiée de mots à cette instance du StopWordDictionary. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Ajoute la collection spécifiée de mots à cette instance du StopWordDictionary. |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Supprime la collection spécifiée de mots de cette instance du StopWordDictionary. |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Supprime la collection spécifiée de mots de cette instance du StopWordDictionary. |
|
|  | [contains(String word)](#contains-java.lang.String-) | Détermine si un objet StopWordDictionary contient le mot spécifié. |
|
|  | [clear()](#clear--) | Supprime tous les mots d'un objet StopWordDictionary. |
|
|  | [iterator()](#iterator--) | Retourne un itérateur qui parcourt la collection. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtient le nombre de mots vides contenus dans le StopWordDictionary.


**Returns:**
int - Le nombre de mots vides dans le dictionnaire.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Ajoute la collection spécifiée de mots à cette instance du StopWordDictionary.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mots | java.lang.Iterable<java.lang.String> | La collection de mots à ajouter au dictionnaire. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Ajoute la collection spécifiée de mots à cette instance du StopWordDictionary.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mots | java.lang.String[] | La collection de mots à ajouter au dictionnaire. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Supprime la collection spécifiée de mots de cette instance du StopWordDictionary.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mots | java.lang.Iterable<java.lang.String> | La collection de mots à supprimer. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Supprime la collection spécifiée de mots de cette instance du StopWordDictionary.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mots | java.lang.String[] | La collection de mots à supprimer. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Détermine si un objet StopWordDictionary contient le mot spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mot | java.lang.String | Le mot à rechercher dans l'objet StopWordDictionary. |
|

**Returns:**
boolean - true si l'objet StopWordDictionary contient le mot spécifié ; sinon, false.

### clear() {#clear--}
```
public abstract void clear()
```


Supprime tous les mots d'un objet StopWordDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourne un itérateur qui parcourt la collection.


**Returns:**
java.util.Iterator<java.lang.String> - Un itérateur qui peut être utilisé pour parcourir la collection.

