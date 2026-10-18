---
title: "StopWordDictionary"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Define la interfaz de un diccionario de palabras vacías."
type: docs
weight: 22
url: /es/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Define la interfaz de un diccionario de palabras vacías.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCount()](#getCount--) | Obtiene el número de palabras vacías contenidas en el StopWordDictionary. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Agrega la colección especificada de palabras a esta instancia del StopWordDictionary. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Agrega la colección especificada de palabras a esta instancia del StopWordDictionary. |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Elimina la colección especificada de palabras de esta instancia del StopWordDictionary. |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Elimina la colección especificada de palabras de esta instancia del StopWordDictionary. |
|
|  | [contains(String word)](#contains-java.lang.String-) | Determina si un objeto StopWordDictionary contiene la palabra especificada. |
|
|  | [clear()](#clear--) | Elimina todas las palabras de un objeto StopWordDictionary. |
|
|  | [iterator()](#iterator--) | Devuelve un iterador que recorre la colección. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el número de palabras vacías contenidas en el StopWordDictionary.


**Returns:**
int - El número de palabras vacías en el diccionario.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Agrega la colección especificada de palabras a esta instancia del StopWordDictionary.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabras | java.lang.Iterable<java.lang.String> | La colección de palabras para agregar al diccionario. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Agrega la colección especificada de palabras a esta instancia del StopWordDictionary.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabras | java.lang.String[] | La colección de palabras para agregar al diccionario. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Elimina la colección especificada de palabras de esta instancia del StopWordDictionary.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabras | java.lang.Iterable<java.lang.String> | La colección de palabras a eliminar. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Elimina la colección especificada de palabras de esta instancia del StopWordDictionary.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabras | java.lang.String[] | La colección de palabras a eliminar. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Determina si un objeto StopWordDictionary contiene la palabra especificada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabra | java.lang.String | La palabra a localizar en el objeto StopWordDictionary. |
|

**Returns:**
boolean - true si el objeto StopWordDictionary contiene la palabra especificada; de lo contrario, false.

### clear() {#clear--}
```
public abstract void clear()
```


Elimina todas las palabras de un objeto StopWordDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Devuelve un iterador que recorre la colección.


**Returns:**
java.util.Iterator<java.lang.String> - Un iterador que puede usarse para iterar a través de la colección.

