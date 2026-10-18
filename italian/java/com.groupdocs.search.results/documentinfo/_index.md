---
title: "DocumentInfo"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un descrittore per un documento indicizzato."
type: docs
weight: 11
url: /it/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Rappresenta un descrittore per un documento indicizzato.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [toString()](#toString--) | Restituisce una  System.String  che rappresenta l'attuale  DocumentInfo . |
|
|  | [getFilePath()](#getFilePath--) | Ottiene il percorso del file indicizzato da file o la chiave del documento indicizzato da stream o struttura. |
|
|  | [getFileType()](#getFileType--) | Ottiene il tipo di file. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Restituisce la famiglia di formati del documento. |
|
|  | [getInnerPath()](#getInnerPath--) | Ottiene il percorso interno per l'elemento del documento contenitore. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Ottiene le parti del percorso interno per l'elemento del documento contenitore. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Ottiene il tipo di origine del documento. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | Ottiene l'indicatore di errore di indicizzazione. |
|
|  | [serialize()](#serialize--) | Serializza l'istanza corrente in un array di byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserializza un'istanza da un array di byte. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Restituisce una  System.String  che rappresenta l'attuale  DocumentInfo .


**Returns:**
java.lang.String - Una  System.String  che rappresenta l'attuale  DocumentInfo .

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Ottiene il percorso del file indicizzato da file o la chiave del documento indicizzato da stream o struttura.


**Returns:**
java.lang.String - Il percorso del file o la chiave del documento.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Ottiene il tipo di file.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Restituisce la famiglia di formati del documento.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Ottiene il percorso interno per l'elemento del documento contenitore.


**Returns:**
java.lang.String - Il percorso interno.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Ottiene le parti del percorso interno per l'elemento del documento contenitore.


**Returns:**
java.lang.String[] - Le parti del percorso interno.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Ottiene il tipo di origine del documento.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


Ottiene l'indicatore di errore di indicizzazione.


**Returns:**
boolean - L'indicatore di errore di indicizzazione.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serializza l'istanza corrente in un array di byte.


**Returns:**
byte[] - Un array di byte che rappresenta l'istanza corrente.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Deserializza un'istanza da un array di byte.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | array | byte[] | Un array di byte da cui deserializzare. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

