---
title: "FoundImageFrame"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un fotogramma immagine trovato."
type: docs
weight: 16
url: /it/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Rappresenta un fotogramma immagine trovato.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Ottiene le informazioni del documento. |
|
|  | [getImageIndex()](#getImageIndex--) | Ottiene il numero ordinale dell'immagine nel documento. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Restituisce l'indice del fotogramma nell'immagine. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Ottiene il numero di bit non corrispondenti nell'hash dell'immagine. |
|
|  | [toString()](#toString--) | Restituisce un  System.String  che rappresenta il corrente  FoundImageFrame . |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Ottiene le informazioni del documento.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Ottiene il numero ordinale dell'immagine nel documento.


**Returns:**
int - Il numero ordinale dell'immagine nel documento.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Restituisce l'indice del fotogramma nell'immagine.


**Returns:**
int - L'indice del fotogramma nell'immagine.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Ottiene il numero di bit non corrispondenti nell'hash dell'immagine.


**Returns:**
int - Il numero di bit non corrispondenti nell'hash dell'immagine.

### toString() {#toString--}
```
public abstract String toString()
```


Restituisce un  System.String  che rappresenta il corrente  FoundImageFrame .


**Returns:**
java.lang.String - Un  System.String  che rappresenta il corrente  FoundImageFrame .

