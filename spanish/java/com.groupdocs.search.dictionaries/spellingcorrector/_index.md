---
title: "SpellingCorrector"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Define la interfaz de un corrector ortográfico para términos en una consulta."
type: docs
weight: 21
url: /es/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Define la interfaz de un corrector ortográfico para términos en una consulta.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCount()](#getCount--) | Obtiene el número de palabras contenidas en este SpellingCorrector. |
|
|  | [getWords()](#getWords--) | Obtiene la colección de palabras que está actualmente contenida en este SpellingCorrector. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Agrega la colección especificada de palabras a esta instancia del SpellingCorrector. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Agrega la colección especificada de palabras a esta instancia del SpellingCorrector. |
|
|  | [clear()](#clear--) | Elimina todas las palabras de un objeto SpellingCorrector. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el número de palabras contenidas en este SpellingCorrector.


**Returns:**
int - El número de palabras contenidas en este SpellingCorrector.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Obtiene la colección de palabras que está actualmente contenida en este SpellingCorrector.


**Returns:**
java.lang.String[] - La colección de palabras.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Agrega la colección especificada de palabras a esta instancia del SpellingCorrector.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabras | java.lang.Iterable<java.lang.String> | La colección de palabras para agregar al diccionario. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Agrega la colección especificada de palabras a esta instancia del SpellingCorrector.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | palabras | java.lang.String[] | La colección de palabras para agregar al diccionario. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Elimina todas las palabras de un objeto SpellingCorrector.


