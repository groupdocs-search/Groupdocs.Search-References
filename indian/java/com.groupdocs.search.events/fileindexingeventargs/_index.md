---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ अनुक्रमण शुरू होने की घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

दस्तावेज़ अनुक्रमण शुरू होने की घटना के लिए तर्क दर्शाता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDocument()](#getDocument--) | दस्तावेज़ प्राप्त करता है। |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | दस्तावेज़ का पूर्ण पथ प्राप्त करता है। |
|
|  | [getDocumentKey()](#getDocumentKey--) | दस्तावेज़ कुंजी प्राप्त करता है। |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | एक मान प्राप्त करता है जो दर्शाता है कि दस्तावेज़ का इंडेक्सिंग छोड़ देना चाहिए। |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | एक मान सेट करता है जो दर्शाता है कि दस्तावेज़ का इंडेक्सिंग छोड़ देना चाहिए। |
|
|  | [getEncoding()](#getEncoding--) | दस्तावेज़ की एन्कोडिंग प्राप्त करता है। |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | दस्तावेज़ की एन्कोडिंग सेट करता है। |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | कस्टम टेक्स्ट एक्सट्रैक्टर प्राप्त करता है। |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | कस्टम टेक्स्ट एक्सट्रैक्टर सेट करता है। |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | दस्तावेज़ के अतिरिक्त फ़ील्ड प्राप्त करता है। |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | दस्तावेज़ के अतिरिक्त फ़ील्ड सेट करता है। |
|
|  | [getAttributes()](#getAttributes--) | दस्तावेज़ के गुण प्राप्त करता है। |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | दस्तावेज़ के गुण सेट करें। |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


दस्तावेज़ प्राप्त करता है।


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


दस्तावेज़ का पूर्ण पथ प्राप्त करता है।


**Returns:**
java.lang.String - दस्तावेज़ का पूर्ण पथ।

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


दस्तावेज़ कुंजी प्राप्त करता है।


**Returns:**
java.lang.String - दस्तावेज़ कुंजी।

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


एक मान प्राप्त करता है जो दर्शाता है कि दस्तावेज़ का इंडेक्सिंग छोड़ देना चाहिए।


**Returns:**
boolean - एक मान जो दर्शाता है कि दस्तावेज़ का इंडेक्सिंग छोड़ देना चाहिए।

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि दस्तावेज़ का इंडेक्सिंग छोड़ देना चाहिए।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि दस्तावेज़ का इंडेक्सिंग छोड़ देना चाहिए। |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


दस्तावेज़ की एन्कोडिंग प्राप्त करता है।


**Returns:**
java.lang.String - दस्तावेज़ की एन्कोडिंग।

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


दस्तावेज़ की एन्कोडिंग सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | दस्तावेज़ की एन्कोडिंग। |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


कस्टम टेक्स्ट एक्सट्रैक्टर प्राप्त करता है।


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


कस्टम टेक्स्ट एक्सट्रैक्टर सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | कस्टम टेक्स्ट एक्सट्रैक्टर। |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


दस्तावेज़ के अतिरिक्त फ़ील्ड प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.DocumentField[] - दस्तावेज़ के अतिरिक्त फ़ील्ड।

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


दस्तावेज़ के अतिरिक्त फ़ील्ड सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | दस्तावेज़ के अतिरिक्त फ़ील्ड। |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


दस्तावेज़ के गुण प्राप्त करता है।


**Returns:**
java.lang.String[] - दस्तावेज़ के गुण।

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


दस्तावेज़ के गुण सेट करें।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String[] | दस्तावेज़ के गुण। |
|

