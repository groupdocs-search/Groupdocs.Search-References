---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Définit l'interface d'un dictionnaire d'homophones hétérographes."
type: docs
weight: 18
url: /fr/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Définit l'interface d'un dictionnaire d'homophones hétérographes.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCount()](#getCount--) | Obtient le nombre de mots contenus dans ce  HomophoneDictionary . |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Ajoute la collection spécifiée de groupes d'homophones à cette instance du  HomophoneDictionary . |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Ajoute la collection spécifiée de groupes d'homophones à cette instance du  HomophoneDictionary . |
|
|  | [clear()](#clear--) | Supprime tous les mots d'un objet  HomophoneDictionary . |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Obtient les homophones du mot spécifié. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Obtient tous les groupes d'homophones auxquels le mot spécifié appartient. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Obtient tous les groupes d'homophones contenus dans ce dictionnaire. |
|
|  | [iterator()](#iterator--) | Retourne un itérateur qui parcourt la collection. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtient le nombre de mots contenus dans ce  HomophoneDictionary .


**Returns:**
int - Le nombre de mots.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Ajoute la collection spécifiée de groupes d'homophones à cette instance du  HomophoneDictionary .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | La collection de groupes d'homophones à ajouter au dictionnaire. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Ajoute la collection spécifiée de groupes d'homophones à cette instance du  HomophoneDictionary .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | La collection de groupes d'homophones à ajouter au dictionnaire. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Supprime tous les mots d'un objet  HomophoneDictionary .


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Obtient les homophones du mot spécifié. Le tableau résultant ne contient pas le mot original.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mot | java.lang.String | Le mot pour suggérer les homophones. |
|

**Returns:**
java.lang.String[] - Les homophones pour le mot spécifié ou tableau vide si l'objet  HomophoneDictionary  ne contient pas le mot spécifié.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Obtient tous les groupes d'homophones auxquels le mot spécifié appartient.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mot | java.lang.String | Le mot pour obtenir des groupes d'homophones. |
|

**Returns:**
java.lang.String[][] - Tous les groupes d'homophones auxquels le mot spécifié appartient.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Obtient tous les groupes d'homophones contenus dans ce dictionnaire.


**Returns:**
java.lang.String[][] - Tous les groupes d'homophones.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourne un itérateur qui parcourt la collection.


**Returns:**
java.util.Iterator<java.lang.String> - Un itérateur qui peut être utilisé pour parcourir la collection.

