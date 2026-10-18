---
title: "दस्तावेज़"
second_title: "GroupDocs.Search for Java API Reference"
description: "फ़ाइल सिस्टम स्ट्रीम या संरचना से इंडेक्स में जोड़े गए दस्तावेज़ों के लिए बेस क्लास का प्रतिनिधित्व करता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

फ़ाइल सिस्टम, स्ट्रीम या संरचना से इंडेक्स में जोड़े गए दस्तावेज़ों के लिए बेस क्लास का प्रतिनिधित्व करता है। विभिन्न स्रोत प्रकारों से दस्तावेज़ बनाने के लिए स्थैतिक मेथड्स शामिल हैं।


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | दस्तावेज़ स्रोत प्रकार प्राप्त करता है। |
|
|  | [getDocumentKey()](#getDocumentKey--) | इंडेक्स के भीतर दस्तावेज़ की पहचान के लिए उपयोग की जाने वाली दस्तावेज़ कुंजी प्राप्त करता है। |
|
|  | [isLazy()](#isLazy--) | यह दर्शाने वाला मान प्राप्त करता है कि दस्तावेज़ आवश्यकतानुसार लोड किया गया है या नहीं। |
|
|  | [getModificationDate()](#getModificationDate--) | दस्तावेज़ की अंतिम संशोधन तिथि प्राप्त करता है। |
|
|  | [getExtension()](#getExtension--) | इस दस्तावेज़ प्रकार के लिए उपयोग किए जाने वाले एक्सटेंशन को प्राप्त करता है। |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | दस्तावेज़ के अतिरिक्त फ़ील्ड प्राप्त करता है। |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | दस्तावेज़ के अतिरिक्त फ़ील्ड सेट करता है। |
|
|  | [getAttributes()](#getAttributes--) | दस्तावेज़ के गुण प्राप्त करता है। |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | दस्तावेज़ के गुण सेट करता है। |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | फ़ाइल से एक दस्तावेज़ बनाता है। |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | स्ट्रीम से एक दस्तावेज़ बनाता है। |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | टेक्स्ट फ़ील्ड्स की एरे वाली संरचना से एक दस्तावेज़ बनाता है। |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | लेज़ी-लोडेड दस्तावेज़ बनाता है। |
|
|  | [toString()](#toString--) | वर्तमान  Document  को दर्शाने वाला  java.lang.String  लौटाता है। |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


दस्तावेज़ स्रोत प्रकार प्राप्त करता है।


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


इंडेक्स के भीतर दस्तावेज़ की पहचान के लिए उपयोग की जाने वाली दस्तावेज़ कुंजी प्राप्त करता है।


**Returns:**
java.lang.String - इंडेक्स के भीतर दस्तावेज़ की पहचान के लिए उपयोग की जाने वाली दस्तावेज़ कुंजी।

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


यह दर्शाने वाला मान प्राप्त करता है कि दस्तावेज़ आवश्यकतानुसार लोड किया गया है या नहीं।


**Returns:**
boolean - यह दर्शाने वाला मान कि दस्तावेज़ आवश्यकतानुसार लोड किया गया है या नहीं।

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


दस्तावेज़ की अंतिम संशोधन तिथि प्राप्त करता है।


**Returns:**
java.util.Date - दस्तावेज़ की अंतिम संशोधन तिथि।

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


इस दस्तावेज़ प्रकार के लिए उपयोग किए जाने वाले एक्सटेंशन को प्राप्त करता है।


**Returns:**
java.lang.String - इस दस्तावेज़ प्रकार के लिए उपयोग किया गया एक्सटेंशन।

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


दस्तावेज़ के अतिरिक्त फ़ील्ड प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.DocumentField[] - दस्तावेज़ के अतिरिक्त फ़ील्ड।

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


दस्तावेज़ के अतिरिक्त फ़ील्ड सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | दस्तावेज़ के अतिरिक्त फ़ील्ड। |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


दस्तावेज़ के गुण प्राप्त करता है।


**Returns:**
java.lang.String[] - दस्तावेज़ के गुण।

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


दस्तावेज़ के गुण सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String[] | दस्तावेज़ के गुण। |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


फ़ाइल से एक दस्तावेज़ बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | दस्तावेज़ फ़ाइल पथ। |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


स्ट्रीम से एक दस्तावेज़ बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़कुंजी | java.lang.String | दस्तावेज़ कुंजी। |
|
|  | संशोधनतारीख | java.util.Date | दस्तावेज़ संशोधन तिथि। |
|
|  | एक्सटेंशन | java.lang.String | दस्तावेज़ एक्सटेंशन। |
|
|  | स्ट्रीम | java.io.InputStream | दस्तावेज़ स्ट्रीम। |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


टेक्स्ट फ़ील्ड्स की एरे वाली संरचना से एक दस्तावेज़ बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़कुंजी | java.lang.String | दस्तावेज़ कुंजी। |
|
|  | संशोधनतारीख | java.util.Date | दस्तावेज़ संशोधन तिथि। |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | दस्तावेज़ फ़ील्ड। |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


लेज़ी-लोडेड दस्तावेज़ बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | दस्तावेज़ स्रोत प्रकार। यह मान लोड किए गए दस्तावेज़ के प्रकार से मेल खाना चाहिए। |
|
|  | दस्तावेज़कुंजी | java.lang.String | दस्तावेज़ कुंजी। यह मान लोड किए गए दस्तावेज़ की कुंजी से मेल खाना चाहिए। |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | दस्तावेज़ लोडर। |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


वर्तमान  Document  को दर्शाने वाला  java.lang.String  लौटाता है।


**Returns:**
java.lang.String - एक  java.lang.String  जो वर्तमान  दस्तावेज़ को दर्शाता है।

