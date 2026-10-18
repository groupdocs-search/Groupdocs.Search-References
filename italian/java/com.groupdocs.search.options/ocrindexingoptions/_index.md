---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per l'elaborazione OCR e l'indicizzazione del testo riconosciuto."
type: docs
weight: 31
url: /it/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Fornisce opzioni per l'elaborazione OCR e l'indicizzazione del testo riconosciuto.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Ottiene un valore che indica se riconoscere il testo in file immagine separati. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Imposta un valore che indica se riconoscere il testo in file immagine separati. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Ottiene un valore che indica se riconoscere il testo in immagini che sono elementi di un contenitore (ad esempio, immagini in un archivio ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Imposta un valore che indica se riconoscere il testo in immagini che sono elementi di un contenitore (ad esempio, immagini in un archivio ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Ottiene un valore che indica se riconoscere il testo in immagini incorporate (ad esempio, immagini in un documento DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Imposta un valore che indica se riconoscere il testo in immagini incorporate (ad esempio, immagini in un documento DOCX). |
|
|  | [getOcrConnector()](#getOcrConnector--) | Ottiene un connettore OCR utilizzato per l'elaborazione OCR. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Imposta un connettore OCR utilizzato per l'elaborazione OCR. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Ottiene un valore che indica se riconoscere il testo in file immagine separati. Il valore predefinito è false.


**Returns:**
boolean - Un valore che indica se riconoscere il testo in file immagine separati.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Imposta un valore che indica se riconoscere il testo in file immagine separati. Il valore predefinito è false.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se riconoscere il testo in file immagine separati. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Ottiene un valore che indica se riconoscere il testo in immagini che sono elementi di un contenitore (ad esempio, immagini in un archivio ZIP). Il valore predefinito è false.


**Returns:**
boolean - Un valore che indica se riconoscere il testo in immagini che sono elementi di un contenitore.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Imposta un valore che indica se riconoscere il testo in immagini che sono elementi di un contenitore (ad esempio, immagini in un archivio ZIP). Il valore predefinito è false.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se riconoscere il testo in immagini che sono elementi di un contenitore. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Ottiene un valore che indica se riconoscere il testo in immagini incorporate (ad esempio, immagini in un documento DOCX). Il valore predefinito è false.


**Returns:**
boolean - Un valore che indica se riconoscere il testo in immagini incorporate.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Imposta un valore che indica se riconoscere il testo in immagini incorporate (ad esempio, immagini in un documento DOCX). Il valore predefinito è false.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se riconoscere il testo in immagini incorporate. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Ottiene un connettore OCR utilizzato per l'elaborazione OCR. Il valore predefinito è null, il che significa che non viene utilizzato alcun OCR.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Imposta un connettore OCR utilizzato per l'elaborazione OCR. Il valore predefinito è null, il che significa che non viene utilizzato alcun OCR.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Un connettore OCR utilizzato per l'elaborazione OCR. |
|

