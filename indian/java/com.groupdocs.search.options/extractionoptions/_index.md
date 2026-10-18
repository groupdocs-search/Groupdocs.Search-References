---
title: "ExtractionOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ों से डेटा निकालने के लिए विकल्प प्रदान करता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

दस्तावेज़ों से डेटा निकालने के लिए विकल्प प्रदान करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | ExtractionOptions क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | ExtractionOptions क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | ExtractionOptions क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | कस्टम टेक्स्ट एक्सट्रैक्टर प्राप्त करता है। |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | कस्टम टेक्स्ट एक्सट्रैक्टर सेट करता है या सेट करता है। |
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
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


ExtractionOptions क्लास का एक नया उदाहरण प्रारंभ करता है।


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


ExtractionOptions क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


ExtractionOptions क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | विकल्प। |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | कस्टम एक्सट्रैक्टर। |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | ocr कनेक्टर। |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


कस्टम टेक्स्ट एक्सट्रैक्टर प्राप्त करता है। डिफ़ॉल्ट मान null है।


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


कस्टम टेक्स्ट एक्सट्रैक्टर सेट करता है या सेट करता है। डिफ़ॉल्ट मान null है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | कस्टम टेक्स्ट एक्सट्रैक्टर। |
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
