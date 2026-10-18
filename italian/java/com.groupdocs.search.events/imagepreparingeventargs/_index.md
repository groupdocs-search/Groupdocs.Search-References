---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di avvio della preparazione di un'immagine."
type: docs
weight: 15
url: /it/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Rappresenta gli argomenti per l'evento di avvio della preparazione di un'immagine.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Restituisce la chiave del documento. |
|
|  | [getInnerPath()](#getInnerPath--) | Ottiene il percorso interno di un documento annidato. |
|
|  | [getImageIndex()](#getImageIndex--) | Ottiene il numero ordinale dell'immagine nel documento. |
|
|  | [getImageFrames()](#getImageFrames--) | Ottiene i fotogrammi dell'immagine. |
|
|  | [getImageStream()](#getImageStream--) | Ottiene lo stream dell'immagine. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Restituisce la chiave del documento.


**Returns:**
java.lang.String - La chiave del documento.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Ottiene il percorso interno di un documento annidato.


**Returns:**
java.lang.String[] - Il percorso interno di un documento annidato.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Ottiene il numero ordinale dell'immagine nel documento.


**Returns:**
int - Il numero ordinale dell'immagine nel documento.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Ottiene i fotogrammi dell'immagine.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - I fotogrammi dell'immagine.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Ottiene lo stream dell'immagine.


**Returns:**
java.io.InputStream - Lo stream dell'immagine.

