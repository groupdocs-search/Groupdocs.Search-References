---
title: "Documento"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta la classe base per i documenti aggiunti a un indice da flusso o struttura del file system."
type: docs
weight: 13
url: /it/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Rappresenta la classe base per i documenti aggiunti a un indice dal file system, dallo stream o dalla struttura. Contiene metodi statici per creare documenti da diversi tipi di sorgenti.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Ottiene il tipo di origine del documento. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Ottiene la chiave del documento utilizzata per identificare il documento all'interno di un indice. |
|
|  | [isLazy()](#isLazy--) | Ottiene un valore che indica se il documento è caricato su richiesta o meno. |
|
|  | [getModificationDate()](#getModificationDate--) | Ottiene la data dell'ultima modifica del documento. |
|
|  | [getExtension()](#getExtension--) | Ottiene l'estensione utilizzata per questo tipo di documento. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Ottiene i campi aggiuntivi del documento. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Imposta i campi aggiuntivi del documento. |
|
|  | [getAttributes()](#getAttributes--) | Ottiene gli attributi del documento. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Imposta gli attributi del documento. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Crea un documento da un file. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Crea un documento da uno stream. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Crea un documento da una struttura che è un array di campi di testo. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Crea un documento caricato pigramente. |
|
|  | [toString()](#toString--) | Restituisce una  java.lang.String  che rappresenta l'attuale  Documento . |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Ottiene il tipo di origine del documento.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Ottiene la chiave del documento utilizzata per identificare il documento all'interno di un indice.


**Returns:**
java.lang.String - La chiave del documento utilizzata per identificare il documento all'interno di un indice.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Ottiene un valore che indica se il documento è caricato su richiesta o meno.


**Returns:**
boolean - Un valore che indica se il documento è caricato su richiesta o meno.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Ottiene la data dell'ultima modifica del documento.


**Returns:**
java.util.Date - La data dell'ultima modifica del documento.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Ottiene l'estensione utilizzata per questo tipo di documento.


**Returns:**
java.lang.String - L'estensione utilizzata per questo tipo di documento.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Ottiene i campi aggiuntivi del documento.


**Returns:**
com.groupdocs.search.common.DocumentField[] - I campi aggiuntivi del documento.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Imposta i campi aggiuntivi del documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | I campi aggiuntivi per il documento. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Ottiene gli attributi del documento.


**Returns:**
java.lang.String[] - Gli attributi del documento.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Imposta gli attributi del documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String[] | Gli attributi del documento. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Crea un documento da un file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file del documento. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Crea un documento da uno stream.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentKey | java.lang.String | La chiave del documento. |
|
|  | modificationDate | java.util.Date | La data di modifica del documento. |
|
|  | extension | java.lang.String | L'estensione del documento. |
|
|  | stream | java.io.InputStream | Il flusso del documento. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Crea un documento da una struttura che è un array di campi di testo.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentKey | java.lang.String | La chiave del documento. |
|
|  | modificationDate | java.util.Date | La data di modifica del documento. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | I campi del documento. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Crea un documento caricato pigramente.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | Il tipo di origine del documento. Questo valore deve corrispondere al tipo del documento caricato. |
|
|  | documentKey | java.lang.String | La chiave del documento. Questo valore deve corrispondere alla chiave del documento caricato. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | Il caricatore del documento. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Restituisce una  java.lang.String  che rappresenta l'attuale  Documento .


**Returns:**
java.lang.String - Una java.lang.String che rappresenta il Document corrente.

