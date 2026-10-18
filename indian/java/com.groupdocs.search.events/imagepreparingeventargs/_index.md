---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "छवि तैयार करने की शुरुआत की घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

छवि तैयार करने की शुरुआत की घटना के लिए तर्क दर्शाता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | दस्तावेज़ कुंजी प्राप्त करता है। |
|
|  | [getInnerPath()](#getInnerPath--) | नेस्टेड दस्तावेज़ का आंतरिक पथ प्राप्त करता है। |
|
|  | [getImageIndex()](#getImageIndex--) | दस्तावेज़ में छवि का क्रमांक प्राप्त करता है। |
|
|  | [getImageFrames()](#getImageFrames--) | छवि फ्रेम प्राप्त करता है। |
|
|  | [getImageStream()](#getImageStream--) | छवि स्ट्रीम प्राप्त करता है। |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


दस्तावेज़ कुंजी प्राप्त करता है।


**Returns:**
java.lang.String - दस्तावेज़ कुंजी।

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


नेस्टेड दस्तावेज़ का आंतरिक पथ प्राप्त करता है।


**Returns:**
java.lang.String[] - नेस्टेड दस्तावेज़ का आंतरिक पथ।

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


दस्तावेज़ में छवि का क्रमांक प्राप्त करता है।


**Returns:**
int - दस्तावेज़ में छवि का क्रमांक।

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


छवि फ्रेम प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.ImageFrame[] - छवि फ्रेम।

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


छवि स्ट्रीम प्राप्त करता है।


**Returns:**
java.io.InputStream - छवि स्ट्रीम।

