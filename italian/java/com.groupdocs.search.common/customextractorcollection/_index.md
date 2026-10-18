---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Contiene una raccolta di estrattori personalizzati."
type: docs
weight: 13
url: /it/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Contiene una collezione di estrattori personalizzati. Se la collezione contiene un estrattore per qualche estensione di file coperta dagli estrattori integrati, allora questo estrattore verrà usato al posto di quello integrato.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [size()](#size--) | Restituisce il numero di estrattori contenuti nella collezione. |
|
|  | [isReadOnly()](#isReadOnly--) | Ottiene un valore che indica se la raccolta è di sola lettura. |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore per questa collezione. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Aggiunge un estrattore alla collezione. |
|
|  | [clear()](#clear--) | Rimuove tutti gli estrattori dalla collezione. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Determina se la collezione contiene un estrattore specifico. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Copia gli elementi della collezione in un array, iniziando da un indice specifico dell'array. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Rimuove un estrattore dalla collezione. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Restituisce il numero di estrattori contenuti nella collezione.


**Returns:**
int - Il numero di estrattori contenuti nella collezione.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Ottiene un valore che indica se la raccolta è di sola lettura.


**Returns:**
boolean - Un valore che indica se la collezione è di sola lettura.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Restituisce un iteratore per questa collezione.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - Un oggetto iteratore che può essere usato per iterare attraverso la collezione.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Aggiunge un estrattore alla collezione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'estrattore da aggiungere alla collezione. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Rimuove tutti gli estrattori dalla collezione.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Determina se la collezione contiene un estrattore specifico.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'estrattore da individuare nella collezione. |
|

**Returns:**
boolean -  true  se  elemento  è trovato nella collezione; altrimenti,  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Copia gli elementi della collezione in un array, iniziando da un indice specifico dell'array.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | L'array monodimensionale che è la destinazione degli elementi copiati dalla collezione. L'array deve avere indicizzazione basata su zero. |
|
|  | arrayIndex | int | L'indice basato su zero nell'array a partire dal quale inizia la copia. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Rimuove un estrattore dalla collezione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'estrattore da rimuovere dalla collezione. |
|

**Returns:**
boolean -  true  se  estrattore  è stato rimosso con successo dalla collezione; altrimenti,  false . Questo metodo restituisce anche  false  se  estrattore  non è trovato nella collezione originale.

