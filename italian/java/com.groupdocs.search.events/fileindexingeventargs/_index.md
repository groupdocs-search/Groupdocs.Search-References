---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per l'evento di avvio dell'indicizzazione di un documento."
type: docs
weight: 14
url: /it/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Rappresenta gli argomenti per l'evento di avvio dell'indicizzazione di un documento.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDocument()](#getDocument--) | Restituisce il documento. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Restituisce il percorso completo del documento. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Restituisce la chiave del documento. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Restituisce un valore che indica se l'indicizzazione del documento deve essere saltata. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Imposta un valore che indica se l'indicizzazione del documento deve essere saltata. |
|
|  | [getEncoding()](#getEncoding--) | Restituisce la codifica del documento. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Imposta la codifica del documento. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Ottiene l'estrattore di testo personalizzato. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Imposta l'estrattore di testo personalizzato. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Ottiene i campi aggiuntivi del documento. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Imposta i campi aggiuntivi del documento. |
|
|  | [getAttributes()](#getAttributes--) | Ottiene gli attributi del documento. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Imposta gli attributi del documento. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Restituisce il documento.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Restituisce il percorso completo del documento.


**Returns:**
java.lang.String - Il percorso completo del documento.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Restituisce la chiave del documento.


**Returns:**
java.lang.String - La chiave del documento.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Restituisce un valore che indica se l'indicizzazione del documento deve essere saltata.


**Returns:**
boolean - Un valore che indica se l'indicizzazione del documento deve essere saltata.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Imposta un valore che indica se l'indicizzazione del documento deve essere saltata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Un valore che indica se l'indicizzazione del documento deve essere saltata. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Restituisce la codifica del documento.


**Returns:**
java.lang.String - La codifica del documento.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Imposta la codifica del documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String | La codifica del documento. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Ottiene l'estrattore di testo personalizzato.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Imposta l'estrattore di testo personalizzato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | L'estrattore di testo personalizzato. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Ottiene i campi aggiuntivi del documento.


**Returns:**
com.groupdocs.search.common.DocumentField[] - I campi aggiuntivi del documento.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Imposta i campi aggiuntivi del documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | I campi aggiuntivi per il documento. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Ottiene gli attributi del documento.


**Returns:**
java.lang.String[] - Gli attributi del documento.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Imposta gli attributi del documento.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | java.lang.String[] | Gli attributi del documento. |
|

