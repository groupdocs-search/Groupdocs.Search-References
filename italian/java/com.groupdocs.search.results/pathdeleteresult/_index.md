---
title: "PathDeleteResult"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta il risultato dell'operazione di eliminazione di un file o cartella indicizzati da un indice."
type: docs
weight: 18
url: /it/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Rappresenta il risultato dell'operazione di eliminazione di un file o cartella indicizzati da un indice.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Restituisce l'indicatore di successo dell'operazione di eliminazione. |
|
|  | [getError()](#getError--) | Restituisce una descrizione dell'errore di eliminazione. |
|
|  | [getPath()](#getPath--) | Restituisce il percorso del file o della cartella da eliminare. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Restituisce l'indicatore di successo dell'operazione di eliminazione.


**Returns:**
boolean -  true  se l'operazione di eliminazione ha avuto successo; altrimenti, restituisce  false .

### getError() {#getError--}
```
public final String getError()
```


Restituisce una descrizione dell'errore di eliminazione.


**Returns:**
java.lang.String - Una descrizione dell'errore di eliminazione.

### getPath() {#getPath--}
```
public final String getPath()
```


Restituisce il percorso del file o della cartella da eliminare.


**Returns:**
java.lang.String - Il percorso del file o della cartella da eliminare.

