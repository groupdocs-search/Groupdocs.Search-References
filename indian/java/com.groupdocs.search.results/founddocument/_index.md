---
title: "FoundDocument"
second_title: "GroupDocs.Search for Java API Reference"
description: "पाया गया दस्तावेज़ का प्रतिनिधित्व करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

पाया गया दस्तावेज़ का प्रतिनिधित्व करता है।


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | दस्तावेज़ जानकारी को प्राप्त करता है। |
|
|  | [getRelevance()](#getRelevance--) | खोज परिणाम की प्रासंगिकता प्राप्त करता है। |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | पाए गए आवृत्तियों की संख्या को प्राप्त करता है। |
|
|  | [getFoundFields()](#getFoundFields--) | पाए गए दस्तावेज़ फ़ील्ड प्राप्त करता है। |
|
|  | [getTerms()](#getTerms--) | पाए गए शब्दों को प्राप्त करता है। |
|
|  | [getTermSequences()](#getTermSequences--) | पाए गए शब्द अनुक्रमों को प्राप्त करता है। |
|
|  | [getAttributes()](#getAttributes--) | पाए गए दस्तावेज़ से जुड़े गुण प्राप्त करता है। |
|
|  | [toString()](#toString--) | पाए गए दस्तावेज़ का स्ट्रिंग प्रतिनिधित्व लौटाता है। |
|
|  | [serialize()](#serialize--) | वर्तमान इंस्टेंस को बाइट एरे में सीरियलाइज़ करता है। |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | बाइट एरे से एक इंस्टेंस को डीसीरियलाइज़ करता है। |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


दस्तावेज़ जानकारी को प्राप्त करता है।


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


खोज परिणाम की प्रासंगिकता प्राप्त करता है।


**Returns:**
double - खोज परिणाम की प्रासंगिकता।

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


पाए गए आवृत्तियों की संख्या को प्राप्त करता है।


**Returns:**
int - पाए गए आवृत्तियों की संख्या।

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


पाए गए दस्तावेज़ फ़ील्ड प्राप्त करता है।


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - पाए गए दस्तावेज़ फ़ील्ड।

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


पाए गए शब्द प्राप्त करता है। मान प्रत्येक बार जब प्रॉपर्टी तक पहुँचते हैं तो मूल्यांकित किया जाता है।


**Returns:**
java.lang.String[] - पाए गए शब्द।

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


पाए गए शब्द अनुक्रमों को प्राप्त करता है।


**Returns:**
java.lang.String[][] - पाए गए शब्द अनुक्रम।

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


पाए गए दस्तावेज़ से जुड़े गुण प्राप्त करता है। गुण प्राप्त करने के लिए खोज विकल्पों में संबंधित विकल्प को सक्षम होना चाहिए।


**Returns:**
java.lang.String[] - पाए गए दस्तावेज़ से जुड़े गुण।

### toString() {#toString--}
```
public abstract String toString()
```


पाए गए दस्तावेज़ का स्ट्रिंग प्रतिनिधित्व लौटाता है।


**Returns:**
java.lang.String - एक स्ट्रिंग जो पाए गए दस्तावेज़ का प्रतिनिधित्व करती है।

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


वर्तमान इंस्टेंस को बाइट एरे में सीरियलाइज़ करता है।


**Returns:**
byte[] - वर्तमान इंस्टेंस को दर्शाने वाला बाइट एरे।

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


बाइट एरे से एक इंस्टेंस को डीसीरियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | एरे | byte[] | डीसीरियलाइज़ करने के लिए बाइट एरे। |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

