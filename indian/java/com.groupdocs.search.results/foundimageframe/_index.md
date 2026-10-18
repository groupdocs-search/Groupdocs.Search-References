---
title: "FoundImageFrame"
second_title: "GroupDocs.Search for Java API Reference"
description: "पाई गई छवि फ्रेम का प्रतिनिधित्व करता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

पाई गई छवि फ्रेम का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | दस्तावेज़ जानकारी को प्राप्त करता है। |
|
|  | [getImageIndex()](#getImageIndex--) | दस्तावेज़ में छवि का क्रमांक प्राप्त करता है। |
|
|  | [getFrameIndex()](#getFrameIndex--) | छवि में फ्रेम का इंडेक्स प्राप्त करता है। |
|
|  | [getHashDifferences()](#getHashDifferences--) | इमेज हैश में असंगत बिट्स की संख्या को प्राप्त करता है। |
|
|  | [toString()](#toString--) | वर्तमान  FoundImageFrame  का प्रतिनिधित्व करने वाला एक  System.String  लौटाता है। |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


दस्तावेज़ जानकारी को प्राप्त करता है।


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


दस्तावेज़ में छवि का क्रमांक प्राप्त करता है।


**Returns:**
int - दस्तावेज़ में छवि का क्रमांक।

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


छवि में फ्रेम का इंडेक्स प्राप्त करता है।


**Returns:**
int - छवि में फ्रेम का इंडेक्स।

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


इमेज हैश में असंगत बिट्स की संख्या को प्राप्त करता है।


**Returns:**
int - इमेज हैश में असंगत बिट्स की संख्या।

### toString() {#toString--}
```
public abstract String toString()
```


वर्तमान  FoundImageFrame  का प्रतिनिधित्व करने वाला एक  System.String  लौटाता है।


**Returns:**
java.lang.String - एक  System.String  जो वर्तमान  FoundImageFrame  का प्रतिनिधित्व करता है।

