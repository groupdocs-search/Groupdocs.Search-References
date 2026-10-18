---
title: "TextOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स से दस्तावेज़ टेक्स्ट प्राप्त करने के लिए विकल्प प्रदान करता है।"
type: docs
weight: 41
url: /hi/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

इंडेक्स से दस्तावेज़ टेक्स्ट प्राप्त करने के लिए विकल्प प्रदान करता है।


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [TextOptions()](#TextOptions--) |   TextOptions  क्लास का एक नया उदाहरण आरंभ करता है। |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) |   TextOptions  क्लास का एक नया उदाहरण आरंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | इंडेक्सिंग के लिए उपयोग किए गए कस्टम टेक्स्ट एक्सट्रैक्टर को प्राप्त करता है। |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | इंडेक्सिंग के लिए उपयोग किए गए कस्टम टेक्स्ट एक्सट्रैक्टर को सेट करता है। |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | इंडेक्सिंग के लिए उपयोग किए गए अतिरिक्त दस्तावेज़ फ़ील्ड प्राप्त करता है। |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | इंडेक्सिंग के लिए उपयोग किए गए अतिरिक्त दस्तावेज़ फ़ील्ड सेट करता है। |
|
|  | [getCancellation()](#getCancellation--) | रद्द करने वाले ऑब्जेक्ट को प्राप्त करता है। |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | रद्द करने वाले ऑब्जेक्ट को सेट करता है। |
|
|  | [getGenerateHead()](#getGenerateHead--) | आउटपुट HTML में Head टैग उत्पन्न होता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | आउटपुट HTML में Head टैग उत्पन्न होता है या नहीं, यह दर्शाने वाला मान सेट करता है। |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


  TextOptions  क्लास का एक नया उदाहरण आरंभ करता है।


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


  TextOptions  क्लास का एक नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


इंडेक्सिंग के लिए उपयोग किए गए कस्टम टेक्स्ट एक्सट्रैक्टर को प्राप्त करता है। डिफ़ॉल्ट मान null है। ध्यान दें कि यह मान केवल तब उपयोग किया जाता है जब दस्तावेज़ टेक्स्ट को इंडेक्स में सहेजा नहीं गया हो।


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


इंडेक्सिंग के लिए उपयोग किए गए कस्टम टेक्स्ट एक्सट्रैक्टर को सेट करता है। डिफ़ॉल्ट मान null है। ध्यान दें कि यह मान केवल तब उपयोग किया जाता है जब दस्तावेज़ टेक्स्ट को इंडेक्स में सहेजा नहीं गया हो।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | इंडेक्सिंग के लिए उपयोग किया गया कस्टम टेक्स्ट एक्सट्रैक्टर। |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


इंडेक्सिंग के लिए उपयोग किए गए अतिरिक्त दस्तावेज़ फ़ील्ड को प्राप्त करता है। डिफ़ॉल्ट मान null है। ध्यान दें कि यह मान केवल तब उपयोग किया जाता है जब दस्तावेज़ टेक्स्ट को इंडेक्स में सहेजा नहीं गया हो।


**Returns:**
com.groupdocs.search.common.DocumentField[] - इंडेक्सिंग के लिए उपयोग किए गए अतिरिक्त दस्तावेज़ फ़ील्ड।

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


इंडेक्सिंग के लिए उपयोग किए गए अतिरिक्त दस्तावेज़ फ़ील्ड को सेट करता है। डिफ़ॉल्ट मान null है। ध्यान दें कि यह मान केवल तब उपयोग किया जाता है जब दस्तावेज़ टेक्स्ट को इंडेक्स में सहेजा नहीं गया हो।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | इंडेक्सिंग के लिए उपयोग किए गए अतिरिक्त दस्तावेज़ फ़ील्ड। |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


रद्द करने वाले ऑब्जेक्ट को प्राप्त करता है। डिफ़ॉल्ट मान null है।


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


रद्द करने वाले ऑब्जेक्ट को सेट करता है। डिफ़ॉल्ट मान null है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | रद्दीकरण वस्तु। |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


आउटपुट HTML में Head टैग उत्पन्न होता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। डिफ़ॉल्ट मान true है।


**Returns:**
boolean - आउटपुट HTML में Head टैग उत्पन्न होता है या नहीं, यह दर्शाने वाला मान।

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


आउटपुट HTML में Head टैग उत्पन्न होता है या नहीं, यह दर्शाने वाला मान सेट करता है। डिफ़ॉल्ट मान true है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | आउटपुट HTML में Head टैग उत्पन्न होता है या नहीं, यह दर्शाने वाला मान। |
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
