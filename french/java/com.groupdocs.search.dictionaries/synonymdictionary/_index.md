---
title: "SynonymDictionary"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Définit l'interface d'un dictionnaire de synonymes."
type: docs
weight: 23
url: /fr/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Définit l'interface d'un dictionnaire de synonymes.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCount()](#getCount--) | Obtient le nombre de mots contenus dans ce  SynonymDictionary . |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Ajoute la collection spécifiée de groupes de synonymes à cette instance du  SynonymDictionary . |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Ajoute la collection spécifiée de groupes de synonymes à cette instance du  SynonymDictionary . |
|
|  | [clear()](#clear--) | Supprime tous les mots de cet objet  SynonymDictionary . |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Obtient les synonymes du mot spécifié. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Obtient tous les groupes de synonymes auxquels appartient le mot spécifié. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Obtient tous les groupes de synonymes contenus dans ce dictionnaire. |
|
|  | [iterator()](#iterator--) | Retourne un itérateur qui parcourt la collection. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtient le nombre de mots contenus dans ce  SynonymDictionary .


**Returns:**
int - Le nombre de mots contenus dans ce  SynonymDictionary .

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Ajoute la collection spécifiée de groupes de synonymes à cette instance du  SynonymDictionary .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | synonymes | java.lang.Iterable<java.lang.String[]> | La collection de groupes de synonymes à ajouter au dictionnaire. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Ajoute la collection spécifiée de groupes de synonymes à cette instance du  SynonymDictionary .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | synonymes | java.lang.String[][] | La collection de groupes de synonymes à ajouter au dictionnaire. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Supprime tous les mots de cet objet  SynonymDictionary .


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Obtient les synonymes du mot spécifié. Le tableau résultant ne contient pas le mot original.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mot | java.lang.String | Le mot pour suggérer les synonymes. |
|

**Returns:**
java.lang.String[] - Les synonymes du mot spécifié ou tableau vide si l'objet  SynonymDictionary  ne contient pas le mot spécifié.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Obtient tous les groupes de synonymes auxquels appartient le mot spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mot | java.lang.String | Le mot pour obtenir des groupes de synonymes. |
|

**Returns:**
java.lang.String[][] - Tous les groupes de synonymes auxquels le mot spécifié appartient.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Obtient tous les groupes de synonymes contenus dans ce dictionnaire.


**Returns:**
java.lang.String[][] - Tous les groupes de synonymes.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourne un itérateur qui parcourt la collection.


**Returns:**
java.util.Iterator<java.lang.String> - Un itérateur qui peut être utilisé pour parcourir la collection.

