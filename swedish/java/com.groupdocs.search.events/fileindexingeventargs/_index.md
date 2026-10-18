---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelsen när en dokumentindexering startar."
type: docs
weight: 14
url: /sv/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Representerar argument för händelsen när en dokumentindexering startar.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDocument()](#getDocument--) | Hämtar dokumentet. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Hämtar dokumentets fullständiga sökväg. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Hämtar dokumentnyckeln. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Hämtar ett värde som indikerar att indexering av dokumentet ska hoppas över. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Ställer in ett värde som indikerar att indexering av dokumentet ska hoppas över. |
|
|  | [getEncoding()](#getEncoding--) | Hämtar kodningen för dokumentet. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Ställer in kodningen för dokumentet. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Hämtar den anpassade textutdragaren. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Ställer in den anpassade textextrahören. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Hämtar de ytterligare fälten för dokumentet. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Ställer in de ytterligare fälten för dokumentet. |
|
|  | [getAttributes()](#getAttributes--) | Hämtar dokumentets attribut. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Ställ in attributen för dokumentet. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Hämtar dokumentet.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Hämtar dokumentets fullständiga sökväg.


**Returns:**
java.lang.String - Dokumentets fullständiga sökväg.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Hämtar dokumentnyckeln.


**Returns:**
java.lang.String - Dokumentnyckeln.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Hämtar ett värde som indikerar att indexering av dokumentet ska hoppas över.


**Returns:**
boolean - Ett värde som indikerar att indexering av dokumentet ska hoppas över.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Ställer in ett värde som indikerar att indexering av dokumentet ska hoppas över.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar att indexering av dokumentet ska hoppas över. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Hämtar kodningen för dokumentet.


**Returns:**
java.lang.String - Kodningen av dokumentet.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Ställer in kodningen för dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Kodningen av dokumentet. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Hämtar den anpassade textutdragaren.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Ställer in den anpassade textextrahören.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Den anpassade textutdragaren. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Hämtar de ytterligare fälten för dokumentet.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De ytterligare fälten för dokumentet.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Ställer in de ytterligare fälten för dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | De ytterligare fälten för dokumentet. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Hämtar dokumentets attribut.


**Returns:**
java.lang.String[] - Dokumentets attribut.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Ställ in attributen för dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String[] | Dokumentets attribut. |
|

