---
title: "IndexingOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्सिंग ऑपरेशन के लिए विकल्प प्रदान करता है।"
type: docs
weight: 25
url: /hi/java/com.groupdocs.search.options/indexingoptions/
---
**Inheritance:**
java.lang.Object
```
public class IndexingOptions
```

इंडेक्सिंग ऑपरेशन के लिए विकल्प प्रदान करता है।


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [IndexingOptions()](#IndexingOptions--) | IndexingOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [IndexingOptions(Object data)](#IndexingOptions-java.lang.Object-) | IndexingOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getThreads()](#getThreads--) | इंडेक्सिंग के लिए उपयोग किए जाने वाले थ्रेड्स की संख्या प्राप्त करता है। |
|
|  | [setThreads(int value)](#setThreads-int-) | इंडेक्सिंग के लिए उपयोग किए जाने वाले थ्रेड्स की संख्या सेट करता है। |
|
|  | [isAsync()](#isAsync--) | ऑपरेशन को असिंक्रोनस रूप से करने के फ़्लैग को प्राप्त करता है। |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | ऑपरेशन को असिंक्रोनस रूप से करने के फ़्लैग को सेट करता है। |
|
|  | [getCancellation()](#getCancellation--) | ऑपरेशन रद्द करने वाले ऑब्जेक्ट को प्राप्त करता है। |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | ऑपरेशन रद्द करने वाले ऑब्जेक्ट को सेट करता है। |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | एक मान प्राप्त करता है जो दर्शाता है कि एन्कोडिंग को स्वचालित रूप से पता करना है या नहीं। |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | एक मान सेट करता है जो दर्शाता है कि एन्कोडिंग को स्वचालित रूप से पता करना है या नहीं। |
|
|  | [getEncoding()](#getEncoding--) | टेक्स्ट दस्तावेज़ों से पाठ निकालने के लिए उपयोग किए जाने वाले एन्कोडिंग को प्राप्त करता है। |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | टेक्स्ट दस्तावेज़ों से टेक्स्ट निकालने के लिए उपयोग की जाने वाली एन्कोडिंग सेट करता है। |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | यदि संभव हो तो टेक्स्ट निष्कर्षण के लिए रॉ मोड उपयोग किया जाता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | यदि संभव हो तो टेक्स्ट निष्कर्षण के लिए रॉ मोड उपयोग किया जाता है या नहीं, यह दर्शाने वाला मान सेट करता है। |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | मेटाडेटा फ़ील्ड्स को इंडेक्स करने के विकल्प प्राप्त करता है। |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | OCR प्रोसेसिंग और पहचाने गए टेक्स्ट को इंडेक्स करने के विकल्प प्राप्त करता है। |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | रिवर्स इमेज सर्च के लिए इमेज इंडेक्सिंग विकल्प प्राप्त करता है। |
|
| [getCore()](#getCore--) |  |
### IndexingOptions() {#IndexingOptions--}
```
public IndexingOptions()
```


IndexingOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


### IndexingOptions(Object data) {#IndexingOptions-java.lang.Object-}
```
public IndexingOptions(Object data)
```


IndexingOptions क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


इंडेक्सिंग के लिए उपयोग की जाने वाली थ्रेड्स की संख्या प्राप्त करता है। डिफ़ॉल्ट मान 1 है।


**Returns:**
int - इंडेक्सिंग के लिए उपयोग की जाने वाली थ्रेड्स की संख्या।

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


इंडेक्सिंग के लिए उपयोग की जाने वाली थ्रेड्स की संख्या सेट करता है। डिफ़ॉल्ट मान 1 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | इंडेक्सिंग के लिए उपयोग की जाने वाली थ्रेड्स की संख्या। |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


ऑपरेशन को असिंक्रोनस रूप से करने का फ़्लैग प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - ऑपरेशन को असिंक्रोनस रूप से करने का फ़्लैग।

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


ऑपरेशन को असिंक्रोनस रूप से करने का फ़्लैग सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | ऑपरेशन को असिंक्रोनस रूप से करने का फ़्लैग। |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


ऑपरेशन रद्द करने वाले ऑब्जेक्ट को प्राप्त करता है। डिफ़ॉल्ट मान null है।


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


ऑपरेशन रद्द करने वाले ऑब्जेक्ट को सेट करता है। डिफ़ॉल्ट मान null है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | ऑपरेशन रद्द करने वाला ऑब्जेक्ट। |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


एन्कोडिंग को स्वचालित रूप से पहचानना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - एन्कोडिंग को स्वचालित रूप से पहचानना है या नहीं, यह दर्शाने वाला मान।

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


एन्कोडिंग को स्वचालित रूप से पहचानना है या नहीं, यह दर्शाने वाला मान सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एन्कोडिंग को स्वचालित रूप से पहचानना है या नहीं, यह दर्शाने वाला मान। |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


टेक्स्ट दस्तावेज़ों से टेक्स्ट निकालने के लिए उपयोग की जाने वाली एन्कोडिंग प्राप्त करता है। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि डिफ़ॉल्ट एन्कोडिंग UTF-8 उपयोग की जाती है। यदि AutoDetectEncoding true है तो यह मान डिफ़ॉल्ट एन्कोडिंग के रूप में उपयोग किया जाता है।


**Returns:**
java.lang.String - टेक्स्ट दस्तावेज़ों से टेक्स्ट निकालने के लिए उपयोग की जाने वाली एन्कोडिंग।

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


टेक्स्ट दस्तावेज़ों से टेक्स्ट निकालने के लिए उपयोग की जाने वाली एन्कोडिंग सेट करता है। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि डिफ़ॉल्ट एन्कोडिंग UTF-8 उपयोग की जाती है। यदि AutoDetectEncoding true है तो यह मान डिफ़ॉल्ट एन्कोडिंग के रूप में उपयोग किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | टेक्स्ट दस्तावेज़ों से टेक्स्ट निकालने के लिए उपयोग की जाने वाली एन्कोडिंग। |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


एक मान प्राप्त करता है जो दर्शाता है कि यदि संभव हो तो टेक्स्ट निष्कर्षण के लिए रॉ मोड उपयोग किया जाता है या नहीं। डिफ़ॉल्ट मान true है। रॉ मोड इंडेक्सिंग गति को काफी बढ़ा सकता है, लेकिन सामान्य मोड निकाले गए टेक्स्ट के फ़ॉर्मेटिंग को सुधारता है।


**Returns:**
boolean - एक मान जो दर्शाता है कि यदि संभव हो तो टेक्स्ट निष्कर्षण के लिए रॉ मोड उपयोग किया जाता है या नहीं।

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि यदि संभव हो तो टेक्स्ट निष्कर्षण के लिए रॉ मोड उपयोग किया जाता है या नहीं। डिफ़ॉल्ट मान true है। रॉ मोड इंडेक्सिंग गति को काफी बढ़ा सकता है, लेकिन सामान्य मोड निकाले गए टेक्स्ट के फ़ॉर्मेटिंग को सुधारता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि यदि संभव हो तो टेक्स्ट निष्कर्षण के लिए रॉ मोड उपयोग किया जाता है या नहीं। |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


मेटाडेटा फ़ील्ड्स को इंडेक्स करने के विकल्प प्राप्त करता है।


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


OCR प्रोसेसिंग और पहचाने गए टेक्स्ट को इंडेक्स करने के विकल्प प्राप्त करता है।


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


रिवर्स इमेज सर्च के लिए इमेज इंडेक्सिंग विकल्प प्राप्त करता है।


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
