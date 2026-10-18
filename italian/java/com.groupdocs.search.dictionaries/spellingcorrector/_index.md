---
title: "SpellingCorrector"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Definisce l'interfaccia di un correttore ortografico per i termini in una query."
type: docs
weight: 21
url: /it/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Definisce l'interfaccia di un correttore ortografico per i termini in una query.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCount()](#getCount--) | Ottiene il numero di parole contenute in questo  SpellingCorrector . |
|
|  | [getWords()](#getWords--) | Ottiene la collezione di parole attualmente contenuta in questo  SpellingCorrector . |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Aggiunge la collezione specificata di parole a questa istanza del  SpellingCorrector . |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Aggiunge la collezione specificata di parole a questa istanza del  SpellingCorrector . |
|
|  | [clear()](#clear--) | Rimuove tutte le parole da un oggetto  SpellingCorrector . |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Ottiene il numero di parole contenute in questo  SpellingCorrector .


**Returns:**
int - Il numero di parole contenute in questo  SpellingCorrector .

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Ottiene la collezione di parole attualmente contenuta in questo  SpellingCorrector .


**Returns:**
java.lang.String[] - La collezione di parole.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Aggiunge la collezione specificata di parole a questa istanza del  SpellingCorrector .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parole | java.lang.Iterable<java.lang.String> | La collezione di parole da aggiungere al dizionario. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Aggiunge la collezione specificata di parole a questa istanza del  SpellingCorrector .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | parole | java.lang.String[] | La collezione di parole da aggiungere al dizionario. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Rimuove tutte le parole da un oggetto  SpellingCorrector .


