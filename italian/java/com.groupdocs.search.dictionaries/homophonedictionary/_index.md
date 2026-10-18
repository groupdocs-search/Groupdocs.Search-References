---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Definisce l'interfaccia di un dizionario di omofoni eterografici."
type: docs
weight: 18
url: /it/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Definisce l'interfaccia di un dizionario di omofoni eterografici.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCount()](#getCount--) | Restituisce il numero di parole contenute in questo  HomophoneDictionary . |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Aggiunge la collezione specificata di gruppi di omofoni a questa istanza del  HomophoneDictionary . |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Aggiunge la collezione specificata di gruppi di omofoni a questa istanza del  HomophoneDictionary . |
|
|  | [clear()](#clear--) | Rimuove tutte le parole da un oggetto  HomophoneDictionary . |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Restituisce gli omofoni per la parola specificata. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Restituisce tutti i gruppi di omofoni a cui appartiene la parola specificata. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Restituisce tutti i gruppi di omofoni contenuti in questo dizionario. |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore che scorre la collezione. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Restituisce il numero di parole contenute in questo  HomophoneDictionary .


**Returns:**
int - Il numero di parole.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Aggiunge la collezione specificata di gruppi di omofoni a questa istanza del  HomophoneDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | omofoni | java.lang.Iterable<java.lang.String[]> | La collezione di gruppi di omofoni da aggiungere al dizionario. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Aggiunge la collezione specificata di gruppi di omofoni a questa istanza del  HomophoneDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | omofoni | java.lang.String[][] | La collezione di gruppi di omofoni da aggiungere al dizionario. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Rimuove tutte le parole da un oggetto  HomophoneDictionary .


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Restituisce gli omofoni per la parola specificata. L'array risultante non contiene la parola originale.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parola | java.lang.String | La parola per suggerire gli omofoni. |
|

**Returns:**
java.lang.String[] - Gli omofoni per la parola specificata o array vuoto se l'oggetto  HomophoneDictionary  non contiene la parola specificata.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Restituisce tutti i gruppi di omofoni a cui appartiene la parola specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parola | java.lang.String | La parola per ottenere gruppi di omofoni. |
|

**Returns:**
java.lang.String[][] - Tutti i gruppi di omofoni a cui appartiene la parola specificata.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Restituisce tutti i gruppi di omofoni contenuti in questo dizionario.


**Returns:**
java.lang.String[][] - Tutti i gruppi di omofoni.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Restituisce un iteratore che scorre la collezione.


**Returns:**
java.util.Iterator<java.lang.String> - Un iteratore che può essere usato per iterare attraverso la collezione.

