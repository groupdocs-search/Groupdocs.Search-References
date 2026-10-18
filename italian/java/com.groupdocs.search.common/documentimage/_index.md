---
title: "DocumentImage"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta i dati dell'immagine del documento."
type: docs
weight: 16
url: /it/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Rappresenta i dati dell'immagine del documento.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Ottiene il numero ordinale dell'immagine nel documento. |
|
|  | [getFields()](#getFields--) | Ottiene i campi estratti. |
|
|  | [getFrames()](#getFrames--) | Ottiene i fotogrammi dell'immagine. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Ottiene il numero ordinale dell'immagine nel documento.


**Returns:**
int - Il numero ordinale dell'immagine nel documento.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Ottiene i campi estratti.


**Returns:**
com.groupdocs.search.common.DocumentField[] - I campi estratti.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Ottiene i fotogrammi dell'immagine.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - I fotogrammi dell'immagine.

