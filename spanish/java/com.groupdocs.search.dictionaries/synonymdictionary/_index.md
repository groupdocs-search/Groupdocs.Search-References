---
title: "SynonymDictionary"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Define la interfaz de un diccionario de sinónimos."
type: docs
weight: 23
url: /es/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Define la interfaz de un diccionario de sinónimos.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCount()](#getCount--) | Obtiene el número de palabras contenidas en este  SynonymDictionary . |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Agrega la colección especificada de grupos de sinónimos a esta instancia del  SynonymDictionary . |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Agrega la colección especificada de grupos de sinónimos a esta instancia del  SynonymDictionary . |
|
|  | [clear()](#clear--) | Elimina todas las palabras de este  SynonymDictionary  objeto. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Obtiene los sinónimos de la palabra especificada. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Obtiene todos los grupos de sinónimos a los que pertenece la palabra especificada. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Obtiene todos los grupos de sinónimos contenidos en este diccionario. |
|
|  | [iterator()](#iterator--) | Devuelve un iterador que recorre la colección. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el número de palabras contenidas en este  SynonymDictionary .


**Returns:**
int - El número de palabras contenidas en este  SynonymDictionary .

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Agrega la colección especificada de grupos de sinónimos a esta instancia del  SynonymDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | sinónimos | java.lang.Iterable<java.lang.String[]> | La colección de grupos de sinónimos para agregar al diccionario. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Agrega la colección especificada de grupos de sinónimos a esta instancia del  SynonymDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | sinónimos | java.lang.String[][] | La colección de grupos de sinónimos para agregar al diccionario. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Elimina todas las palabras de este  SynonymDictionary  objeto.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Obtiene los sinónimos de la palabra especificada. La matriz resultante no contiene la palabra original.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabra | java.lang.String | La palabra para sugerir los sinónimos. |
|

**Returns:**
java.lang.String[] - Los sinónimos de la palabra especificada o una matriz vacía si el  SynonymDictionary  objeto no contiene la palabra especificada.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Obtiene todos los grupos de sinónimos a los que pertenece la palabra especificada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabra | java.lang.String | La palabra para obtener grupos de sinónimos. |
|

**Returns:**
java.lang.String[][] - Todos los grupos de sinónimos a los que pertenece la palabra especificada.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Obtiene todos los grupos de sinónimos contenidos en este diccionario.


**Returns:**
java.lang.String[][] - Todos los grupos de sinónimos.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Devuelve un iterador que recorre la colección.


**Returns:**
java.util.Iterator<java.lang.String> - Un iterador que puede usarse para iterar a través de la colección.

