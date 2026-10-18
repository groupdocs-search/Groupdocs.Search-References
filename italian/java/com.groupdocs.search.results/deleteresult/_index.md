---
title: "DeleteResult"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta il risultato dell'operazione di eliminazione di file o cartelle indicizzati da un indice."
type: docs
weight: 10
url: /it/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Rappresenta il risultato dell'operazione di eliminazione di file o cartelle indicizzati da un indice.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Restituisce i risultati dell'eliminazione di ogni percorso. |
|
|  | [getTotalCount()](#getTotalCount--) | Restituisce il numero totale di percorsi da eliminare. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Restituisce il numero di percorsi eliminati con successo. |
|
|  | [getFailedCount()](#getFailedCount--) | Restituisce il numero di percorsi non eliminati a causa di errori. |
|
|  | [getErrors()](#getErrors--) | Restituisce le descrizioni degli errori di eliminazione. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Restituisce i risultati dell'eliminazione di ogni percorso.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - I risultati dell'eliminazione di ogni percorso.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Restituisce il numero totale di percorsi da eliminare.


**Returns:**
int - Il numero totale di percorsi da eliminare.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Restituisce il numero di percorsi eliminati con successo.


**Returns:**
int - Il numero di percorsi eliminati con successo.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Restituisce il numero di percorsi non eliminati a causa di errori.


**Returns:**
int - Il numero di percorsi non eliminati a causa di errori.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Restituisce le descrizioni degli errori di eliminazione.


**Returns:**
java.lang.String[] - Descrizioni degli errori di eliminazione.

