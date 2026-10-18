---
title: "DateFormatCollection"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta una raccolta di oggetti DateFormat."
type: docs
weight: 14
url: /it/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Rappresenta una collezione di oggetti DateFormat.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Aggiunge un oggetto di formato data alla raccolta. |
|
|  | [clear()](#clear--) | Rimuove tutti gli elementi dalla raccolta. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Determina se la raccolta contiene un elemento specifico. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Copia gli elementi della raccolta in un  Array , a partire da un indice  Array  specifico. |
|
|  | [size()](#size--) | Ottiene il numero di elementi contenuti nella raccolta. |
|
|  | [isReadOnly()](#isReadOnly--) | Ottiene un valore che indica se la raccolta è di sola lettura. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Rimuove la prima occorrenza di un elemento specifico dalla collezione. |
|
|  | [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso la collezione. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Aggiunge un oggetto di formato data alla raccolta.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | L'oggetto formato data da aggiungere alla collezione. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Rimuove tutti gli elementi dalla raccolta.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Determina se la raccolta contiene un elemento specifico.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | L'elemento da individuare nella collezione. |
|

**Returns:**
boolean -  true  se l'elemento è trovato nella collezione; altrimenti,  false .

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Copia gli elementi della raccolta in un  Array , a partire da un indice  Array  specifico.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | L'Array monodimensionale che è la destinazione degli elementi copiati dalla collezione. |
|
|  | arrayIndex | int | L'indice basato su zero nell'array a partire dal quale inizia la copia. |
|

### size() {#size--}
```
public abstract int size()
```


Ottiene il numero di elementi contenuti nella raccolta.


**Returns:**
int - Il numero di elementi contenuti nella collezione.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Ottiene un valore che indica se la raccolta è di sola lettura.


**Returns:**
boolean -  true  se la collezione è di sola lettura; altrimenti,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Rimuove la prima occorrenza di un elemento specifico dalla collezione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | L'elemento da rimuovere dalla collezione. |
|

**Returns:**
boolean -  true  se l'elemento è stato rimosso con successo dalla collezione; altrimenti,  false . Questo metodo restituisce anche  false  se l'elemento non è trovato nella collezione.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Restituisce un enumeratore che itera attraverso la collezione.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - Un enumeratore che può essere usato per iterare attraverso la collezione.

