---
title: "StopWordDictionary"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Definisce l'interfaccia di un dizionario di parole stop."
type: docs
weight: 22
url: /it/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Definisce l'interfaccia di un dizionario di parole stop.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCount()](#getCount--) | Restituisce il numero di parole di stop contenute nel  StopWordDictionary . |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Aggiunge la collezione specificata di parole a questa istanza del  StopWordDictionary . |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Aggiunge la collezione specificata di parole a questa istanza del  StopWordDictionary . |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Rimuove la collezione specificata di parole da questa istanza del  StopWordDictionary . |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Rimuove la collezione specificata di parole da questa istanza del  StopWordDictionary . |
|
|  | [contains(String word)](#contains-java.lang.String-) | Determina se un oggetto  StopWordDictionary  contiene la parola specificata. |
|
|  | [clear()](#clear--) | Rimuove tutte le parole da un oggetto  StopWordDictionary . |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore che scorre la collezione. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Restituisce il numero di parole di stop contenute nel  StopWordDictionary .


**Returns:**
int - Il numero di parole di stop nel dizionario.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Aggiunge la collezione specificata di parole a questa istanza del  StopWordDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parole | java.lang.Iterable<java.lang.String> | La collezione di parole da aggiungere al dizionario. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Aggiunge la collezione specificata di parole a questa istanza del  StopWordDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parole | java.lang.String[] | La collezione di parole da aggiungere al dizionario. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Rimuove la collezione specificata di parole da questa istanza del  StopWordDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parole | java.lang.Iterable<java.lang.String> | La collezione di parole da rimuovere. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Rimuove la collezione specificata di parole da questa istanza del  StopWordDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parole | java.lang.String[] | La collezione di parole da rimuovere. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Determina se un oggetto  StopWordDictionary  contiene la parola specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parola | java.lang.String | La parola da individuare nell'oggetto  StopWordDictionary . |
|

**Returns:**
boolean -  true  se l'oggetto  StopWordDictionary  contiene la parola specificata; altrimenti,  false .

### clear() {#clear--}
```
public abstract void clear()
```


Rimuove tutte le parole da un oggetto  StopWordDictionary .


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Restituisce un iteratore che scorre la collezione.


**Returns:**
java.util.Iterator<java.lang.String> - Un iteratore che può essere usato per iterare attraverso la collezione.

