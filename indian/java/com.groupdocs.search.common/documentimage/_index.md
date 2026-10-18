---
title: "DocumentImage"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक दस्तावेज़ इमेज डेटा का प्रतिनिधित्व करता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

एक दस्तावेज़ इमेज डेटा का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | दस्तावेज़ में छवि का क्रमांक प्राप्त करता है। |
|
|  | [getFields()](#getFields--) | निकाले गए फ़ील्ड प्राप्त करता है। |
|
|  | [getFrames()](#getFrames--) | छवि फ्रेम प्राप्त करता है। |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


दस्तावेज़ में छवि का क्रमांक प्राप्त करता है।


**Returns:**
int - दस्तावेज़ में छवि का क्रमांक।

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


निकाले गए फ़ील्ड प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.DocumentField[] - निकाले गए फ़ील्ड।

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


छवि फ्रेम प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.ImageFrame[] - छवि फ्रेम।

