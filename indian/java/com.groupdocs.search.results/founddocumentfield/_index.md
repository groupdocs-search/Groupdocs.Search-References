---
title: "FoundDocumentField"
second_title: "GroupDocs.Search for Java API Reference"
description: "पाए गए दस्तावेज़ फ़ील्ड का प्रतिनिधित्व करता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

पाए गए दस्तावेज़ फ़ील्ड का प्रतिनिधित्व करता है।


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | फ़ील्ड का नाम प्राप्त करता है। |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | पाए गए आवृत्तियों की संख्या को प्राप्त करता है। |
|
|  | [getTerms()](#getTerms--) | पाए गए शब्दों को प्राप्त करता है। |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | पाए गए शब्दों की आवृत्तियों को प्राप्त करता है। |
|
|  | [getTermSequences()](#getTermSequences--) | पाए गए शब्द अनुक्रमों को प्राप्त करता है। |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | पाए गए शब्द अनुक्रमों की आवृत्तियों को प्राप्त करता है। |
|
|  | [toString()](#toString--) | पाए गए दस्तावेज़ फ़ील्ड का स्ट्रिंग प्रतिनिधित्व लौटाता है। |
|
|  | [serialize()](#serialize--) | वर्तमान इंस्टेंस को बाइट एरे में सीरियलाइज़ करता है। |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | बाइट एरे से एक इंस्टेंस को डीसीरियलाइज़ करता है। |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


फ़ील्ड का नाम प्राप्त करता है।


**Returns:**
java.lang.String - फ़ील्ड नाम।

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


पाए गए आवृत्तियों की संख्या को प्राप्त करता है।


**Returns:**
int - पाए गए आवृत्तियों की संख्या।

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


पाए गए शब्दों को प्राप्त करता है।


**Returns:**
java.lang.String[] - पाए गए शब्द।

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


पाए गए शब्दों की आवृत्तियों को प्राप्त करता है।


**Returns:**
int[] - पाए गए शब्दों की आवृत्तियों।

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


पाए गए शब्द अनुक्रमों को प्राप्त करता है।


**Returns:**
java.lang.String[][] - पाए गए शब्द अनुक्रम।

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


पाए गए शब्द अनुक्रमों की आवृत्तियों को प्राप्त करता है।


**Returns:**
int[] - पाए गए शब्द अनुक्रमों की आवृत्तियों।

### toString() {#toString--}
```
public abstract String toString()
```


पाए गए दस्तावेज़ फ़ील्ड का स्ट्रिंग प्रतिनिधित्व लौटाता है।


**Returns:**
java.lang.String - एक स्ट्रिंग जो पाए गए दस्तावेज़ फ़ील्ड का प्रतिनिधित्व करती है।

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


वर्तमान इंस्टेंस को बाइट एरे में सीरियलाइज़ करता है।


**Returns:**
byte[] - वर्तमान इंस्टेंस को दर्शाने वाला बाइट एरे।

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


बाइट एरे से एक इंस्टेंस को डीसीरियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | एरे | byte[] | डीसीरियलाइज़ करने के लिए बाइट एरे। |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

