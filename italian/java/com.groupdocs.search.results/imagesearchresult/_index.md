---
title: "ImageSearchResult"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta il risultato di una ricerca inversa di immagini."
type: docs
weight: 17
url: /it/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Rappresenta il risultato di una ricerca inversa di immagini.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Restituisce il numero di immagini trovate. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Restituisce l'immagine trovata per indice. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Restituisce il numero di immagini trovate.


**Returns:**
int - Il numero di immagini trovate.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Restituisce l'immagine trovata per indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indice | int | L'indice di un'immagine trovata. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

