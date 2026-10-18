---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्सिंग मेटाडेटा फ़ील्ड्स के लिए विकल्प प्रदान करता है।"
type: docs
weight: 29
url: /hi/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

इंडेक्सिंग मेटाडेटा फ़ील्ड्स के लिए विकल्प प्रदान करता है।


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | एक मान प्राप्त करता है जो दर्शाता है कि खाली फ़ील्ड मानों को इंडेक्स किया जाए या नहीं। |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | एक मान सेट करता है जो दर्शाता है कि खाली फ़ील्ड मानों को इंडेक्स किया जाए या नहीं। |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | एक मान प्राप्त करता है जो दर्शाता है कि खाली फ़ील्ड नामों को इंडेक्स किया जाए या नहीं। |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | एक मान सेट करता है जो दर्शाता है कि खाली फ़ील्ड नामों को इंडेक्स किया जाए या नहीं। |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | डिफ़ॉल्ट फ़ील्ड नाम प्राप्त करता है जो खाली फ़ील्ड नामों को इंडेक्स करने के लिए उपयोग किया जाता है। |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | डिफ़ॉल्ट फ़ील्ड नाम सेट करता है जो खाली फ़ील्ड नामों को इंडेक्स करने के लिए उपयोग किया जाता है। |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | फ़ील्ड के संयुक्त नाम में विभाजक प्राप्त करता है। |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | फ़ील्ड के संयुक्त नाम में विभाजक सेट करता है। |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | फ़ील्ड को इंडेक्स करने के लिए बाइट प्रकार की एरे में मानों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | फ़ील्ड को इंडेक्स करने के लिए बाइट प्रकार की एरे में मानों की अधिकतम संख्या सेट करता है। |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | फ़ील्ड को इंडेक्स करने के लिए इंट प्रकार की एरे में मानों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | फ़ील्ड को इंडेक्स करने के लिए इंट प्रकार की एरे में मानों की अधिकतम संख्या सेट करता है। |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | फ़ील्ड को इंडेक्स करने के लिए लॉन्ग प्रकार की एरे में मानों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | फ़ील्ड को इंडेक्स करने के लिए लॉन्ग प्रकार की एरे में मानों की अधिकतम संख्या सेट करता है। |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | फ़ील्ड को इंडेक्स करने के लिए डबल प्रकार की एरे में मानों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | फ़ील्ड को इंडेक्स करने के लिए डबल प्रकार की एरे में मानों की अधिकतम संख्या सेट करता है। |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | एरे प्रकार के फ़ील्ड में मानों के बीच विभाजक प्राप्त करता है। |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | एरे प्रकार के फ़ील्ड में मानों के बीच विभाजक सेट करता है। |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


एक मान प्राप्त करता है जो दर्शाता है कि खाली फ़ील्ड मानों को इंडेक्स किया जाए या नहीं। डिफ़ॉल्ट मान true है।


**Returns:**
boolean - एक मान जो दर्शाता है कि खाली फ़ील्ड मानों को इंडेक्स किया जाए या नहीं।

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


खाली फ़ील्ड मानों को अनुक्रमित करने के लिए संकेत करने वाला मान सेट करता है या नहीं। डिफ़ॉल्ट मान है true।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | खाली फ़ील्ड मानों को अनुक्रमित करने के लिए संकेत करने वाला मान। |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


खाली फ़ील्ड नामों को अनुक्रमित करने के लिए संकेत करने वाला मान प्राप्त करता है या नहीं। डिफ़ॉल्ट मान है true।


**Returns:**
boolean - खाली फ़ील्ड नामों को अनुक्रमित करने के लिए संकेत करने वाला मान।

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


खाली फ़ील्ड नामों को अनुक्रमित करने के लिए संकेत करने वाला मान सेट करता है या नहीं। डिफ़ॉल्ट मान है true।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | खाली फ़ील्ड नामों को अनुक्रमित करने के लिए संकेत करने वाला मान। |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


खाली फ़ील्ड नामों को अनुक्रमित करने के लिए उपयोग किया जाने वाला डिफ़ॉल्ट फ़ील्ड नाम प्राप्त करता है। डिफ़ॉल्ट मान है "unknown"।


**Returns:**
java.lang.String - खाली फ़ील्ड नामों को अनुक्रमित करने के लिए उपयोग किया जाने वाला डिफ़ॉल्ट फ़ील्ड नाम।

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


खाली फ़ील्ड नामों को अनुक्रमित करने के लिए उपयोग किया जाने वाला डिफ़ॉल्ट फ़ील्ड नाम सेट करता है। डिफ़ॉल्ट मान है "unknown"।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | खाली फ़ील्ड नामों को अनुक्रमित करने के लिए उपयोग किया जाने वाला डिफ़ॉल्ट फ़ील्ड नाम। |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


फ़ील्ड के संयुक्त नाम में विभाजक प्राप्त करता है। डिफ़ॉल्ट मान है "."।


**Returns:**
java.lang.String - फ़ील्ड के संयुक्त नाम में विभाजक।

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


फ़ील्ड के संयुक्त नाम में विभाजक सेट करता है। डिफ़ॉल्ट मान है "."।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | फ़ील्ड के संयुक्त नाम में विभाजक। |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


फ़ील्ड को अनुक्रमित करने के लिए byte प्रकार की एरे में मानों की अधिकतम संख्या प्राप्त करता है। डिफ़ॉल्ट मान है Integer.MAX_VALUE।


**Returns:**
int - फ़ील्ड को अनुक्रमित करने के लिए byte प्रकार की एरे में मानों की अधिकतम संख्या।

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


फ़ील्ड को अनुक्रमित करने के लिए byte प्रकार की एरे में मानों की अधिकतम संख्या सेट करता है। डिफ़ॉल्ट मान है Integer.MAX_VALUE।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | फ़ील्ड को अनुक्रमित करने के लिए byte प्रकार की एरे में मानों की अधिकतम संख्या। |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


फ़ील्ड को अनुक्रमित करने के लिए int प्रकार की एरे में मानों की अधिकतम संख्या प्राप्त करता है। डिफ़ॉल्ट मान है Integer.MAX_VALUE।


**Returns:**
int - फ़ील्ड को अनुक्रमित करने के लिए int प्रकार की एरे में मानों की अधिकतम संख्या।

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


फ़ील्ड को अनुक्रमित करने के लिए int प्रकार की एरे में मानों की अधिकतम संख्या सेट करता है। डिफ़ॉल्ट मान है Integer.MAX_VALUE।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | फ़ील्ड को अनुक्रमित करने के लिए int प्रकार की एरे में मानों की अधिकतम संख्या। |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


फ़ील्ड को अनुक्रमित करने के लिए long प्रकार की एरे में मानों की अधिकतम संख्या प्राप्त करता है। डिफ़ॉल्ट मान है Integer.MAX_VALUE।


**Returns:**
int - फ़ील्ड को अनुक्रमित करने के लिए long प्रकार की एरे में मानों की अधिकतम संख्या।

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


फ़ील्ड को अनुक्रमित करने के लिए long प्रकार की एरे में मानों की अधिकतम संख्या सेट करता है। डिफ़ॉल्ट मान है Integer.MAX_VALUE।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | फ़ील्ड को इंडेक्स करने के लिए long प्रकार की एरे में मानों की अधिकतम संख्या। |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


फ़ील्ड को इंडेक्स करने के लिए double प्रकार की एरे में मानों की अधिकतम संख्या प्राप्त करता है। डिफ़ॉल्ट मान Integer.MAX_VALUE है।


**Returns:**
int - फ़ील्ड को इंडेक्स करने के लिए double प्रकार की एरे में मानों की अधिकतम संख्या।

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


फ़ील्ड को इंडेक्स करने के लिए double प्रकार की एरे में मानों की अधिकतम संख्या सेट करता है। डिफ़ॉल्ट मान Integer.MAX_VALUE है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | फ़ील्ड को इंडेक्स करने के लिए double प्रकार की एरे में मानों की अधिकतम संख्या। |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


एरे प्रकार के फ़ील्ड में मानों के बीच विभाजक प्राप्त करता है। डिफ़ॉल्ट मान स्पेस चिन्ह है।


**Returns:**
java.lang.String - एरे प्रकार के फ़ील्ड में मानों के बीच विभाजक।

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


एरे प्रकार के फ़ील्ड में मानों के बीच विभाजक सेट करता है। डिफ़ॉल्ट मान स्पेस चिन्ह है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | एरे प्रकार के फ़ील्ड में मानों के बीच विभाजक। |
|

