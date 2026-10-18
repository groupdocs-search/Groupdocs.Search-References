---
title: "SearchImage"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un'immagine da cercare."
type: docs
weight: 29
url: /it/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Rappresenta un'immagine da cercare.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Crea un'immagine da un file per la ricerca. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Crea un'immagine da un file per la ricerca. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Crea un'immagine da uno stream per la ricerca. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Crea un'immagine da uno stream per la ricerca. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Crea un'immagine da un file per la ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file immagine. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Crea un'immagine da un file per la ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file immagine. |
|
|  | imageIndex | int | L'indice dell'immagine nelle immagini multipagina. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Crea un'immagine da uno stream per la ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | stream | java.io.InputStream | Lo stream dell'immagine. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Crea un'immagine da uno stream per la ricerca.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | stream | java.io.InputStream | Lo stream dell'immagine. |
|
|  | imageIndex | int | L'indice dell'immagine nelle immagini multipagina. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

