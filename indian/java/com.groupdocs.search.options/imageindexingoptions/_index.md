---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "रिवर्स इमेज सर्च के लिए इमेज इंडेक्सिंग विकल्प प्रदान करता है।"
type: docs
weight: 23
url: /hi/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

रिवर्स इमेज सर्च के लिए इमेज इंडेक्सिंग विकल्प प्रदान करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या अलग-अलग इमेज फ़ाइलों को इंडेक्स किया जाए। |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | एक मान सेट करता है जो दर्शाता है कि क्या अलग-अलग इमेज फ़ाइलों को इंडेक्स किया जाए। |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या कंटेनर में मौजूद इमेज (उदाहरण के लिए, ZIP आर्काइव में इमेज) को इंडेक्स किया जाए। |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | एक मान सेट करता है जो दर्शाता है कि क्या कंटेनर में मौजूद इमेज (उदाहरण के लिए, ZIP आर्काइव में इमेज) को इंडेक्स किया जाए। |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या एम्बेडेड इमेज (उदाहरण के लिए, DOCX दस्तावेज़ में इमेज) को इंडेक्स किया जाए। |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | एक मान सेट करता है जो दर्शाता है कि क्या एम्बेडेड इमेज (उदाहरण के लिए, DOCX दस्तावेज़ में इमेज) को इंडेक्स किया जाए। |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या अलग-अलग इमेज फ़ाइलों को इंडेक्स किया जाए। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - एक मान जो दर्शाता है कि क्या अलग-अलग इमेज फ़ाइलों को इंडेक्स किया जाए।

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि क्या अलग-अलग इमेज फ़ाइलों को इंडेक्स किया जाए। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि क्या अलग-अलग इमेज फ़ाइलों को इंडेक्स किया जाए। |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या कंटेनर में मौजूद इमेज (उदाहरण के लिए, ZIP आर्काइव में इमेज) को इंडेक्स किया जाए। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - एक मान जो दर्शाता है कि क्या कंटेनर में आइटम के रूप में मौजूद छवियों को अनुक्रमित किया जाए।

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि क्या कंटेनर में आइटम के रूप में मौजूद छवियों को अनुक्रमित किया जाए (उदाहरण के लिए, ZIP आर्काइव में छवियां)। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि क्या कंटेनर में आइटम के रूप में मौजूद छवियों को अनुक्रमित किया जाए। |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


एक मान प्राप्त करता है जो दर्शाता है कि क्या एम्बेडेड छवियों को अनुक्रमित किया जाए (उदाहरण के लिए, DOCX दस्तावेज़ में छवियां)। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - एक मान जो दर्शाता है कि क्या एम्बेडेड छवियों को अनुक्रमित किया जाए।

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि क्या एम्बेडेड छवियों को अनुक्रमित किया जाए (उदाहरण के लिए, DOCX दस्तावेज़ में छवियां)। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि क्या एम्बेडेड छवियों को अनुक्रमित किया जाए। |
|

