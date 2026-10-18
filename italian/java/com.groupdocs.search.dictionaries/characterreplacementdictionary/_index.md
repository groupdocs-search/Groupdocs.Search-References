---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Definisce l'interfaccia di un dizionario di sostituzione dei caratteri utilizzato durante il processo di indicizzazione."
type: docs
weight: 16
url: /it/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Definisce l'interfaccia di un dizionario di sostituzione dei caratteri utilizzato durante il processo di indicizzazione. La sostituzione dei caratteri può essere usata, ad esempio, per rimuovere gli accenti dai caratteri accentati o per creare un indice non sensibile al maiuscolo/minuscolo.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCount()](#getCount--) | Ottiene il numero di caratteri contenuti in questo  CharacterReplacementDictionary . |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Aggiunge la collezione specificata di sostituzioni di caratteri a questa istanza del  CharacterReplacementDictionary . |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Aggiunge la collezione specificata di sostituzioni di caratteri a questa istanza del  CharacterReplacementDictionary . |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Rimuove la collezione specificata di sostituzioni di caratteri da questa istanza del  CharacterReplacementDictionary . |
|
|  | [contains(char character)](#contains-char-) | Determina se un oggetto  CharacterReplacementDictionary  contiene una sostituzione per il carattere specificato. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Ottiene una sostituzione per il carattere specificato. |
|
|  | [clear()](#clear--) | Rimuove tutte le sostituzioni di caratteri da un oggetto  CharacterReplacementDictionary . |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore che scorre la collezione. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Ottiene il numero di caratteri contenuti in questo  CharacterReplacementDictionary .


**Returns:**
int - Il numero di caratteri nel dizionario.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Aggiunge la collezione specificata di sostituzioni di caratteri a questa istanza del  CharacterReplacementDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | La collezione di sostituzioni di caratteri da aggiungere al dizionario. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Aggiunge la collezione specificata di sostituzioni di caratteri a questa istanza del  CharacterReplacementDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | La collezione di sostituzioni di caratteri da aggiungere al dizionario. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Rimuove la collezione specificata di sostituzioni di caratteri da questa istanza del  CharacterReplacementDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | caratteri | char[] | La collezione di caratteri da rimuovere. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Determina se un oggetto  CharacterReplacementDictionary  contiene una sostituzione per il carattere specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | carattere | char | Il carattere da individuare nell'oggetto  CharacterReplacementDictionary . |
|

**Returns:**
boolean -  true  se l'oggetto  CharacterReplacementDictionary  contiene il carattere specificato; altrimenti,  false .

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Ottiene una sostituzione per il carattere specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | carattere | char | Il carattere per cui ottenere una sostituzione. |
|

**Returns:**
char - La sostituzione per il carattere specificato.

### clear() {#clear--}
```
public abstract void clear()
```


Rimuove tutte le sostituzioni di caratteri da un oggetto  CharacterReplacementDictionary .


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Restituisce un iteratore che scorre la collezione.


**Returns:**
java.util.Iterator<java.lang.Character> - Un iteratore che può essere usato per iterare attraverso la collezione.

