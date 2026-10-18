---
title: "PasswordDictionary"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Definisce l'interfaccia di un dizionario di password dei documenti."
type: docs
weight: 20
url: /it/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Definisce l'interfaccia di un dizionario di password dei documenti.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nel dizionario. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Ottiene la password per il file. |
|
|  | [clear()](#clear--) | Rimuove tutte le password da questo oggetto  PasswordDictionary  . |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Determina se il dizionario contiene una password per il documento specificato. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Aggiunge una password per un documento al dizionario. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Rimuove una password del documento specificato dal dizionario. |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore che scorre la collezione. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Ottiene il numero di elementi contenuti nel dizionario.


**Returns:**
`int - Il numero di elementi contenuti nel dizionario.`

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Ottiene la password per il file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file. |
|

**Returns:**
`java.lang.String - La password per il file.`

### clear() {#clear--}
```
public abstract void clear()
```


Rimuove tutte le password da questo oggetto  PasswordDictionary  .


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Determina se il dizionario contiene una password per il documento specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file del documento. |
|

**Returns:**
`boolean -  true  se il dizionario contiene una password per il documento; altrimenti,  false .`

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Aggiunge una password per un documento al dizionario.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file del documento. |
|
|  | password | java.lang.String | La password del documento. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Rimuove una password del documento specificato dal dizionario.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file del documento. |
|

**Returns:**
`boolean -  true  se la password è stata rimossa con successo; altrimenti,  false . Questo metodo restituisce anche  false  se  filePath  non è stato trovato nel dizionario.`

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Restituisce un iteratore che scorre la collezione.


**Returns:**
java.util.Iterator<java.lang.String> - Un iteratore che può essere usato per iterare attraverso la collezione.

