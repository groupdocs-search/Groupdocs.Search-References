---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, wenn die Indexierung eines Dokuments startet."
type: docs
weight: 14
url: /de/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Stellt Argumente für das Ereignis dar, wenn die Indexierung eines Dokuments startet.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDocument()](#getDocument--) | Gibt das Dokument zurück. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Gibt den vollständigen Pfad des Dokuments zurück. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Ermittelt den Dokumentenschlüssel. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Liefert einen Wert, der angibt, dass das Indexieren des Dokuments übersprungen werden soll. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Setzt einen Wert, der angibt, dass das Indexieren des Dokuments übersprungen werden soll. |
|
|  | [getEncoding()](#getEncoding--) | Liefert die Kodierung des Dokuments. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Setzt die Kodierung des Dokuments. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Gibt den benutzerdefinierten Text‑Extraktor zurück. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Setzt den benutzerdefinierten Textextraktor. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Liefert die zusätzlichen Felder für das Dokument. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Setzt die zusätzlichen Felder für das Dokument. |
|
|  | [getAttributes()](#getAttributes--) | Liefert die Attribute des Dokuments. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Setzt die Attribute des Dokuments. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Gibt das Dokument zurück.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Gibt den vollständigen Pfad des Dokuments zurück.


**Returns:**
java.lang.String - Der vollständige Pfad des Dokuments.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Ermittelt den Dokumentenschlüssel.


**Returns:**
java.lang.String - Der Dokumentenschlüssel.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Liefert einen Wert, der angibt, dass das Indexieren des Dokuments übersprungen werden soll.


**Returns:**
boolean - Ein Wert, der angibt, dass das Indexieren des Dokuments übersprungen werden soll.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Setzt einen Wert, der angibt, dass das Indexieren des Dokuments übersprungen werden soll.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, dass das Indexieren des Dokuments übersprungen werden soll. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Liefert die Kodierung des Dokuments.


**Returns:**
java.lang.String - Die Kodierung des Dokuments.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Setzt die Kodierung des Dokuments.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Die Kodierung des Dokuments. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Gibt den benutzerdefinierten Text‑Extraktor zurück.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Setzt den benutzerdefinierten Textextraktor.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Der benutzerdefinierte Text‑Extraktor. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Liefert die zusätzlichen Felder für das Dokument.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Die zusätzlichen Felder für das Dokument.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Setzt die zusätzlichen Felder für das Dokument.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Die zusätzlichen Felder für das Dokument. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Liefert die Attribute des Dokuments.


**Returns:**
java.lang.String[] - Die Attribute des Dokuments.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Setzt die Attribute des Dokuments.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String[] | Die Attribute des Dokuments. |
|

