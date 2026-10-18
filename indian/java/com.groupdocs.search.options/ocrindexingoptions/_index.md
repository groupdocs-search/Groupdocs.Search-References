---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "OCR प्रोसेसिंग और पहचाने गए टेक्स्ट को इंडेक्स करने के लिए विकल्प प्रदान करता है।"
type: docs
weight: 31
url: /hi/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

OCR प्रोसेसिंग और पहचाने गए टेक्स्ट को इंडेक्स करने के लिए विकल्प प्रदान करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | एक मान प्राप्त करता है जो यह दर्शाता है कि अलग-अलग छवि फ़ाइलों में पाठ को पहचाना जाए या नहीं। |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | एक मान सेट करता है जो यह दर्शाता है कि अलग-अलग छवि फ़ाइलों में पाठ को पहचाना जाए या नहीं। |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | एक मान प्राप्त करता है जो यह दर्शाता है कि कंटेनर में आइटम के रूप में मौजूद छवियों (उदाहरण के लिए, ZIP संग्रह में छवियों) में पाठ को पहचाना जाए या नहीं। |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | एक मान सेट करता है जो यह दर्शाता है कि कंटेनर में आइटम के रूप में मौजूद छवियों (उदाहरण के लिए, ZIP संग्रह में छवियों) में पाठ को पहचाना जाए या नहीं। |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | एक मान प्राप्त करता है जो यह दर्शाता है कि एम्बेडेड छवियों (उदाहरण के लिए, DOCX दस्तावेज़ में छवियों) में पाठ को पहचाना जाए या नहीं। |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | एक मान सेट करता है जो यह दर्शाता है कि एम्बेडेड छवियों (उदाहरण के लिए, DOCX दस्तावेज़ में छवियों) में पाठ को पहचाना जाए या नहीं। |
|
|  | [getOcrConnector()](#getOcrConnector--) | एक OCR कनेक्टर प्राप्त करता है जो OCR प्रोसेसिंग के लिए उपयोग किया जाता है। |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | एक OCR कनेक्टर सेट करता है जो OCR प्रोसेसिंग के लिए उपयोग किया जाता है। |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि अलग-अलग छवि फ़ाइलों में पाठ को पहचाना जाए या नहीं। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - एक मान जो यह दर्शाता है कि अलग-अलग छवि फ़ाइलों में पाठ को पहचाना जाए या नहीं।

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि अलग-अलग छवि फ़ाइलों में पाठ को पहचाना जाए या नहीं। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो यह दर्शाता है कि अलग-अलग छवि फ़ाइलों में पाठ को पहचाना जाए या नहीं। |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि कंटेनर में आइटम के रूप में मौजूद छवियों (उदाहरण के लिए, ZIP संग्रह में छवियों) में पाठ को पहचाना जाए या नहीं। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - एक मान जो यह दर्शाता है कि कंटेनर में आइटम के रूप में मौजूद छवियों में पाठ को पहचाना जाए या नहीं।

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि कंटेनर में आइटम के रूप में मौजूद छवियों (उदाहरण के लिए, ZIP संग्रह में छवियों) में पाठ को पहचाना जाए या नहीं। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो यह दर्शाता है कि कंटेनर में आइटम के रूप में मौजूद छवियों में पाठ को पहचाना जाए या नहीं। |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि एम्बेडेड छवियों (उदाहरण के लिए, DOCX दस्तावेज़ में छवियों) में पाठ को पहचाना जाए या नहीं। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - एक मान जो यह दर्शाता है कि एम्बेडेड छवियों में पाठ को पहचाना जाए या नहीं।

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि एम्बेडेड छवियों (उदाहरण के लिए, DOCX दस्तावेज़ में छवियों) में पाठ को पहचाना जाए या नहीं। डिफ़ॉल्ट मान null है, जिसका अर्थ है कोई OCR उपयोग नहीं किया गया।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो यह दर्शाता है कि एम्बेडेड छवियों में पाठ को पहचाना जाए या नहीं। |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


एक OCR कनेक्टर प्राप्त करता है जो OCR प्रोसेसिंग के लिए उपयोग किया जाता है। डिफ़ॉल्ट मान null है, जिसका अर्थ है कोई OCR उपयोग नहीं किया गया।


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


एक OCR कनेक्टर सेट करता है जो OCR प्रोसेसिंग के लिए उपयोग किया जाता है। डिफ़ॉल्ट मान null है, जिसका अर्थ है कोई OCR उपयोग नहीं किया गया।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | एक OCR कनेक्टर जो OCR प्रोसेसिंग के लिए उपयोग किया जाता है। |
|

