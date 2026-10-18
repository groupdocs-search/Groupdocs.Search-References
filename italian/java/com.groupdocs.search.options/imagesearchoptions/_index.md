---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per l'operazione di ricerca inversa di immagini."
type: docs
weight: 24
url: /it/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Fornisce opzioni per l'operazione di ricerca inversa di immagini.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | Inizializza una nuova istanza della  ImageSearchOptions  classe. |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Inizializza una nuova istanza della  ImageSearchOptions  classe. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Ottiene il numero massimo di bit non corrispondenti nell'hash dell'immagine. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Imposta il numero massimo di bit non corrispondenti nell'hash dell'immagine. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Ottiene il numero massimo di immagini trovate per una richiesta di ricerca inversa di immagini. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Imposta il numero massimo di immagini trovate per una richiesta di ricerca inversa di immagini. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Ottiene il filtro del documento di ricerca. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Ottiene o imposta il filtro del documento di ricerca. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Inizializza una nuova istanza della  ImageSearchOptions  classe.


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Inizializza una nuova istanza della  ImageSearchOptions  classe.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | java.lang.Object | I dati serializzati. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Ottiene il numero massimo di bit non corrispondenti nell'hash dell'immagine. Il valore predefinito è  5 .


**Returns:**
int - Il numero massimo di bit non corrispondenti nell'hash dell'immagine.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Imposta il numero massimo di bit non corrispondenti nell'hash dell'immagine. Il valore predefinito è 5.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di bit non corrispondenti nell'hash dell'immagine. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Ottiene il numero massimo di immagini trovate per una richiesta di ricerca inversa di immagini. Il valore predefinito è 1000.


**Returns:**
int - Il numero massimo di immagini trovate per una richiesta di ricerca inversa di immagini.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Imposta il numero massimo di immagini trovate per una richiesta di ricerca inversa di immagini. Il valore predefinito è 1000.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di immagini trovate per una richiesta di ricerca inversa di immagini. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Ottiene il filtro dei documenti di ricerca.  SearchDocumentFilter  funziona sulla logica di inclusione. Utilizzare la classe  GroupDocs.Search.Options.SearchDocumentFilter  per creare istanze del filtro dei documenti di ricerca. Il valore predefinito è null, il che significa che tutti i documenti trovati verranno restituiti.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Ottiene o imposta il filtro dei documenti di ricerca.  SearchDocumentFilter  funziona sulla logica di inclusione. Utilizzare la classe  GroupDocs.Search.Options.SearchDocumentFilter  per creare istanze del filtro dei documenti di ricerca. Il valore predefinito è null, il che significa che tutti i documenti trovati verranno restituiti.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Il filtro dei documenti di ricerca. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
