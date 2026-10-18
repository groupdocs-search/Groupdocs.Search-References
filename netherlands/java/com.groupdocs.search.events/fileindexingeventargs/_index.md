---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het evenement voor wanneer een documentindexering start."
type: docs
weight: 14
url: /nl/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Stelt de argumenten voor het evenement voor wanneer een documentindexering start.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDocument()](#getDocument--) | Haalt het document op. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Haalt het volledige pad van het document op. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Haalt de document-sleutel op. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Haalt een waarde op die aangeeft dat de indexering van het document moet worden overgeslagen. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Stelt een waarde in die aangeeft dat de indexering van het document moet worden overgeslagen. |
|
|  | [getEncoding()](#getEncoding--) | Haalt de codering van het document op. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Stelt de codering van het document in. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Haalt de aangepaste tekst-extractor op. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Stelt de aangepaste textextractor in. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Haalt de extra velden voor het document op. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Stelt de extra velden voor het document in. |
|
|  | [getAttributes()](#getAttributes--) | Haalt de attributen van het document op. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Stel de attributen van het document in. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Haalt het document op.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Haalt het volledige pad van het document op.


**Returns:**
java.lang.String - Het volledige pad van het document.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Haalt de document-sleutel op.


**Returns:**
java.lang.String - De document-sleutel.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Haalt een waarde op die aangeeft dat de indexering van het document moet worden overgeslagen.


**Returns:**
boolean - Een waarde die aangeeft dat de indexering van het document moet worden overgeslagen.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Stelt een waarde in die aangeeft dat de indexering van het document moet worden overgeslagen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft dat de indexering van het document moet worden overgeslagen. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Haalt de codering van het document op.


**Returns:**
java.lang.String - De codering van het document.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Stelt de codering van het document in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | De codering van het document. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Haalt de aangepaste tekst-extractor op.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Stelt de aangepaste textextractor in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | De aangepaste tekst-extractor. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Haalt de extra velden voor het document op.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De extra velden voor het document.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Stelt de extra velden voor het document in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | De extra velden voor het document. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Haalt de attributen van het document op.


**Returns:**
java.lang.String[] - De attributen van het document.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Stel de attributen van het document in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String[] | De attributen van het document. |
|

