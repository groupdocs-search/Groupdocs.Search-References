---
title: "SynonymDictionary"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Definisce l'interfaccia di un dizionario di sinonimi."
type: docs
weight: 23
url: /it/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Definisce l'interfaccia di un dizionario di sinonimi.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCount()](#getCount--) | Restituisce il numero di parole contenute in questo SynonymDictionary. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Aggiunge la collezione specificata di gruppi di sinonimi a questa istanza di SynonymDictionary. |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Aggiunge la collezione specificata di gruppi di sinonimi a questa istanza di SynonymDictionary. |
|
|  | [clear()](#clear--) | Rimuove tutte le parole da questo oggetto SynonymDictionary. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Restituisce i sinonimi per la parola specificata. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Restituisce tutti i gruppi di sinonimi a cui appartiene la parola specificata. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Restituisce tutti i gruppi di sinonimi contenuti in questo dizionario. |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore che scorre la collezione. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Restituisce il numero di parole contenute in questo SynonymDictionary.


**Returns:**
int - Il numero di parole contenute in questo SynonymDictionary.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Aggiunge la collezione specificata di gruppi di sinonimi a questa istanza di SynonymDictionary.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | sinonimi | java.lang.Iterable<java.lang.String[]> | La collezione di gruppi di sinonimi da aggiungere al dizionario. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Aggiunge la collezione specificata di gruppi di sinonimi a questa istanza di SynonymDictionary.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | sinonimi | java.lang.String[][] | La collezione di gruppi di sinonimi da aggiungere al dizionario. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Rimuove tutte le parole da questo oggetto SynonymDictionary.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Restituisce i sinonimi per la parola specificata. L'array risultante non contiene la parola originale.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parola | java.lang.String | La parola per suggerire i sinonimi. |
|

**Returns:**
java.lang.String[] - I sinonimi per la parola specificata o array vuoto se l'oggetto SynonymDictionary non contiene la parola specificata.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Restituisce tutti i gruppi di sinonimi a cui appartiene la parola specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parola | java.lang.String | La parola per ottenere gruppi di sinonimi. |
|

**Returns:**
java.lang.String[][] - Tutti i gruppi di sinonimi a cui appartiene la parola specificata.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Restituisce tutti i gruppi di sinonimi contenuti in questo dizionario.


**Returns:**
java.lang.String[][] - Tutti i gruppi di sinonimi.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Restituisce un iteratore che scorre la collezione.


**Returns:**
java.util.Iterator<java.lang.String> - Un iteratore che può essere usato per iterare attraverso la collezione.

