---
title: "AliasDictionary"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Définit l'interface d'un dictionnaire d'alias."
type: docs
weight: 14
url: /fr/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Définit l'interface d'un dictionnaire d'alias.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCount()](#getCount--) | Obtient le nombre d'alias contenus dans l'AliasDictionary. |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Ajoute la collection spécifiée de paires alias/remplacement à cette instance de l'AliasDictionary. |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Ajoute la collection spécifiée de paires alias/remplacement à cette instance de l'AliasDictionary. |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Ajoute la paire spécifiée d'alias et de texte associé à cette instance de l'AliasDictionary. |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Supprime l'alias spécifié d'un objet AliasDictionary. |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Détermine si un objet AliasDictionary contient l'alias spécifié. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Obtient le texte associé à l'alias spécifié. |
|
|  | [clear()](#clear--) | Supprime tous les alias d'un objet AliasDictionary. |
|
|  | [iterator()](#iterator--) | Retourne un itérateur qui parcourt la collection. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtient le nombre d'alias contenus dans l'AliasDictionary.


**Returns:**
int - Le nombre d'alias contenus dans l'AliasDictionary.

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Ajoute la collection spécifiée de paires alias/remplacement à cette instance de l'AliasDictionary.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | paires | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | La collection de paires alias/remplacement à ajouter au dictionnaire. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Ajoute la collection spécifiée de paires alias/remplacement à cette instance de l'AliasDictionary.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | La collection de paires alias/remplacement à ajouter au dictionnaire. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Ajoute la paire spécifiée d'alias et de texte associé à cette instance de l'AliasDictionary.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | alias | java.lang.String | L'alias à ajouter au dictionnaire. |
|
|  | texte | java.lang.String | Le texte à associer à l'alias. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Supprime l'alias spécifié d'un objet AliasDictionary.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | alias | java.lang.String | L'alias à supprimer. |
|

**Returns:**
boolean - Cette méthode renvoie  true  si l'alias est trouvé et supprimé avec succès. Cette méthode renvoie  false  si l'alias n'est pas trouvé dans l'objet  AliasDictionary .

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Détermine si un objet AliasDictionary contient l'alias spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | alias | java.lang.String | L'alias à localiser dans l'objet  AliasDictionary . |
|

**Returns:**
boolean -  true  si l'objet  AliasDictionary  contient l'alias spécifié ; sinon,  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Obtient le texte associé à l'alias spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | alias | java.lang.String | L'alias à localiser dans l'objet  AliasDictionary . |
|

**Returns:**
java.lang.String - Un texte associé à l'alias spécifié ou  null .

### clear() {#clear--}
```
public abstract void clear()
```


Supprime tous les alias d'un objet AliasDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourne un itérateur qui parcourt la collection.


**Returns:**
java.util.Iterator<java.lang.String> - Un itérateur qui peut être utilisé pour parcourir la collection.

