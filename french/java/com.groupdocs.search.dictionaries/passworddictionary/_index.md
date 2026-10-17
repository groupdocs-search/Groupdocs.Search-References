---
title: "PasswordDictionary"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Définit l'interface d'un dictionnaire de mots de passe de documents."
type: docs
weight: 20
url: /fr/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Définit l'interface d'un dictionnaire de mots de passe de documents.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans le dictionnaire. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Obtient le mot de passe du fichier. |
|
|  | [clear()](#clear--) | Supprime tous les mots de passe de cet objet  PasswordDictionary . |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Détermine si le dictionnaire contient un mot de passe pour le document spécifié. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Ajoute un mot de passe pour un document au dictionnaire. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Supprime le mot de passe du document spécifié du dictionnaire. |
|
|  | [iterator()](#iterator--) | Retourne un itérateur qui parcourt la collection. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtient le nombre d'éléments contenus dans le dictionnaire.


**Returns:**
int - Le nombre d'éléments contenus dans le dictionnaire.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Obtient le mot de passe du fichier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier. |
|

**Returns:**
java.lang.String - Le mot de passe du fichier.

### clear() {#clear--}
```
public abstract void clear()
```


Supprime tous les mots de passe de cet objet  PasswordDictionary .


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Détermine si le dictionnaire contient un mot de passe pour le document spécifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier du document. |
|

**Returns:**
boolean -  true  si le dictionnaire contient un mot de passe pour le document ; sinon,  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Ajoute un mot de passe pour un document au dictionnaire.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier du document. |
|
|  | mot de passe | java.lang.String | Le mot de passe du document. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Supprime le mot de passe du document spécifié du dictionnaire.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier du document. |
|

**Returns:**
boolean -  true  si le mot de passe a été supprimé avec succès ; sinon,  false . Cette méthode renvoie également  false  si  filePath  n'a pas été trouvé dans le dictionnaire.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourne un itérateur qui parcourt la collection.


**Returns:**
java.util.Iterator<java.lang.String> - Un itérateur qui peut être utilisé pour parcourir la collection.

