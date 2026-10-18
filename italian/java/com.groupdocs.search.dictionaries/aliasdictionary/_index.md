---
title: "AliasDictionary"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Definisce l'interfaccia di un dizionario di alias."
type: docs
weight: 14
url: /it/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Definisce l'interfaccia di un dizionario di alias.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCount()](#getCount--) | Restituisce il numero di alias contenuti nell' AliasDictionary . |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Aggiunge la collezione specificata di coppie alias/sostituzione a questa istanza dell' AliasDictionary . |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Aggiunge la collezione specificata di coppie alias/sostituzione a questa istanza dell' AliasDictionary . |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Aggiunge la coppia specificata di alias e testo associato a questa istanza dell' AliasDictionary . |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Rimuove l'alias specificato da un oggetto AliasDictionary. |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Determina se un oggetto AliasDictionary contiene l'alias specificato. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Restituisce un testo associato all'alias specificato. |
|
|  | [clear()](#clear--) | Rimuove tutti gli alias da un oggetto AliasDictionary. |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore che scorre la collezione. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Restituisce il numero di alias contenuti nell' AliasDictionary .


**Returns:**
int - Il numero di alias contenuti nell' AliasDictionary .

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Aggiunge la collezione specificata di coppie alias/sostituzione a questa istanza dell' AliasDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | coppie | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | La collezione di coppie alias/sostituzione da aggiungere al dizionario. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Aggiunge la collezione specificata di coppie alias/sostituzione a questa istanza dell' AliasDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | La collezione di coppie alias/sostituzione da aggiungere al dizionario. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Aggiunge la coppia specificata di alias e testo associato a questa istanza dell' AliasDictionary .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | alias | java.lang.String | L'alias da aggiungere al dizionario. |
|
|  | testo | java.lang.String | Il testo da associare all'alias. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Rimuove l'alias specificato da un oggetto AliasDictionary.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | alias | java.lang.String | L'alias da rimuovere. |
|

**Returns:**
boolean - Questo metodo restituisce  true  se l'alias è stato trovato e rimosso correttamente. Questo metodo restituisce  false  se l'alias non è stato trovato nell'oggetto  AliasDictionary .

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Determina se un oggetto AliasDictionary contiene l'alias specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | alias | java.lang.String | L'alias da individuare nell'oggetto  AliasDictionary . |
|

**Returns:**
boolean -  true  se l'oggetto  AliasDictionary  contiene l'alias specificato; altrimenti,  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Restituisce un testo associato all'alias specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | alias | java.lang.String | L'alias da individuare nell'oggetto  AliasDictionary . |
|

**Returns:**
java.lang.String - Un testo associato all'alias specificato o  null .

### clear() {#clear--}
```
public abstract void clear()
```


Rimuove tutti gli alias da un oggetto AliasDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Restituisce un iteratore che scorre la collezione.


**Returns:**
java.util.Iterator<java.lang.String> - Un iteratore che può essere usato per iterare attraverso la collezione.

