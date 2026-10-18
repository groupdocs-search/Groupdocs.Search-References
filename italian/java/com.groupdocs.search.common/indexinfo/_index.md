---
title: "IndexInfo"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Contiene informazioni di base su un indice."
type: docs
weight: 24
url: /it/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Contiene informazioni di base su un indice.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Restituisce l'identificatore univoco dell'indice. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Restituisce il nome completo della cartella dove si trova l'indice. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Restituisce lo stato dell'indice. |
|
|  | [getVersion()](#getVersion--) | Restituisce la versione dell'indice. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Restituisce il numero di segmenti dell'indice. |
|
|  | [getTermCount()](#getTermCount--) | Restituisce il numero di parole nell'indice. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Restituisce l'identificatore univoco dell'indice.


**Returns:**
java.util.UUID - L'identificatore univoco dell'indice.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Restituisce il nome completo della cartella dove si trova l'indice.


**Returns:**
java.lang.String - Il nome completo della cartella dove si trova l'indice.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Restituisce lo stato dell'indice.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Restituisce la versione dell'indice.


**Returns:**
java.lang.String - La versione dell'indice.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Restituisce il numero di segmenti dell'indice.


**Returns:**
int - Il numero di segmenti dell'indice.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Restituisce il numero di parole nell'indice.


**Returns:**
int - Il numero di parole nell'indice.

