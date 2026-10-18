---
title: "HomophoneDictionary"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Define la interfaz de un diccionario de homófonos heterográficos."
type: docs
weight: 18
url: /es/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Define la interfaz de un diccionario de homófonos heterográficos.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCount()](#getCount--) | Obtiene el número de palabras contenidas en este  HomophoneDictionary . |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Añade la colección especificada de grupos de homófonos a esta instancia del  HomophoneDictionary . |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Añade la colección especificada de grupos de homófonos a esta instancia del  HomophoneDictionary . |
|
|  | [clear()](#clear--) | Elimina todas las palabras de un objeto  HomophoneDictionary . |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Obtiene los homófonos de la palabra especificada. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Obtiene todos los grupos de homófonos a los que pertenece la palabra especificada. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Obtiene todos los grupos de homófonos contenidos en este diccionario. |
|
|  | [iterator()](#iterator--) | Devuelve un iterador que recorre la colección. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el número de palabras contenidas en este  HomophoneDictionary .


**Returns:**
int - El número de palabras.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Añade la colección especificada de grupos de homófonos a esta instancia del  HomophoneDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | La colección de grupos de homófonos para añadir al diccionario. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Añade la colección especificada de grupos de homófonos a esta instancia del  HomophoneDictionary .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | La colección de grupos de homófonos para añadir al diccionario. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Elimina todas las palabras de un objeto  HomophoneDictionary .


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Obtiene los homófonos de la palabra especificada. La matriz resultante no contiene la palabra original.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabra | java.lang.String | La palabra para sugerir los homófonos. |
|

**Returns:**
java.lang.String[] - Los homófonos para la palabra especificada o una matriz vacía si el objeto HomophoneDictionary no contiene la palabra especificada.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Obtiene todos los grupos de homófonos a los que pertenece la palabra especificada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabra | java.lang.String | La palabra para obtener grupos de homófonos. |
|

**Returns:**
java.lang.String[][] - Todos los grupos de homófonos a los que pertenece la palabra especificada.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Obtiene todos los grupos de homófonos contenidos en este diccionario.


**Returns:**
java.lang.String[][] - Todos los grupos de homófonos.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Devuelve un iterador que recorre la colección.


**Returns:**
java.util.Iterator<java.lang.String> - Un iterador que puede usarse para iterar a través de la colección.

