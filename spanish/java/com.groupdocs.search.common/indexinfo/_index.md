---
title: "IndexInfo"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Contiene información básica sobre un Índice."
type: docs
weight: 24
url: /es/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Contiene información básica sobre un Índice.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Obtiene el identificador único del índice. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Obtiene el nombre completo de la carpeta donde se encuentra el índice. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Obtiene el estado del índice. |
|
|  | [getVersion()](#getVersion--) | Obtiene la versión del índice. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Obtiene el número de segmentos del índice. |
|
|  | [getTermCount()](#getTermCount--) | Obtiene el número de palabras en el índice. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Obtiene el identificador único del índice.


**Returns:**
java.util.UUID - El identificador único del índice.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Obtiene el nombre completo de la carpeta donde se encuentra el índice.


**Returns:**
java.lang.String - El nombre completo de la carpeta donde se encuentra el índice.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Obtiene el estado del índice.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Obtiene la versión del índice.


**Returns:**
java.lang.String - La versión del índice.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Obtiene el número de segmentos del índice.


**Returns:**
int - El número de segmentos del índice.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Obtiene el número de palabras en el índice.


**Returns:**
int - El número de palabras en el índice.

