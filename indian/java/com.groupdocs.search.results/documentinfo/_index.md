---
title: "DocumentInfo"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक अनुक्रमित दस्तावेज़ के लिए वर्णनकर्ता का प्रतिनिधित्व करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

एक अनुक्रमित दस्तावेज़ के लिए वर्णनकर्ता का प्रतिनिधित्व करता है।


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [toString()](#toString--) | वर्तमान DocumentInfo का प्रतिनिधित्व करने वाली System.String लौटाता है। |
|
|  | [getFilePath()](#getFilePath--) | फ़ाइल से इंडेक्स किए गए फ़ाइल पथ या स्ट्रीम या संरचना से इंडेक्स किए गए दस्तावेज़ कुंजी प्राप्त करता है। |
|
|  | [getFileType()](#getFileType--) | फ़ाइल प्रकार प्राप्त करता है। |
|
|  | [getFormatFamily()](#getFormatFamily--) | दस्तावेज़ फ़ॉर्मेट परिवार प्राप्त करता है। |
|
|  | [getInnerPath()](#getInnerPath--) | कंटेनर दस्तावेज़ आइटम के लिए आंतरिक पथ प्राप्त करता है। |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | कंटेनर दस्तावेज़ आइटम के लिए आंतरिक पथ भाग प्राप्त करता है। |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | दस्तावेज़ स्रोत प्रकार प्राप्त करता है। |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | इंडेक्सिंग त्रुटि संकेतक प्राप्त करता है। |
|
|  | [serialize()](#serialize--) | वर्तमान इंस्टेंस को बाइट एरे में सीरियलाइज़ करता है। |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | बाइट एरे से एक इंस्टेंस को डीसीरियलाइज़ करता है। |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


वर्तमान DocumentInfo का प्रतिनिधित्व करने वाली System.String लौटाता है।


**Returns:**
java.lang.String - वर्तमान DocumentInfo का प्रतिनिधित्व करने वाली System.String।

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


फ़ाइल से इंडेक्स किए गए फ़ाइल पथ या स्ट्रीम या संरचना से इंडेक्स किए गए दस्तावेज़ कुंजी प्राप्त करता है।


**Returns:**
java.lang.String - फ़ाइल पथ या दस्तावेज़ कुंजी।

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


फ़ाइल प्रकार प्राप्त करता है।


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


दस्तावेज़ फ़ॉर्मेट परिवार प्राप्त करता है।


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


कंटेनर दस्तावेज़ आइटम के लिए आंतरिक पथ प्राप्त करता है।


**Returns:**
java.lang.String - आंतरिक पथ।

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


कंटेनर दस्तावेज़ आइटम के लिए आंतरिक पथ भाग प्राप्त करता है।


**Returns:**
java.lang.String[] - आंतरिक पथ भाग।

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


दस्तावेज़ स्रोत प्रकार प्राप्त करता है।


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


इंडेक्सिंग त्रुटि संकेतक प्राप्त करता है।


**Returns:**
boolean - इंडेक्सिंग त्रुटि संकेतक।

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


वर्तमान इंस्टेंस को बाइट एरे में सीरियलाइज़ करता है।


**Returns:**
byte[] - वर्तमान इंस्टेंस को दर्शाने वाला बाइट एरे।

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


बाइट एरे से एक इंस्टेंस को डीसीरियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | एरे | byte[] | डीसीरियलाइज़ करने के लिए बाइट एरे। |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

