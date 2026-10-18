---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "रिवर्स इमेज सर्च ऑपरेशन के लिए विकल्प प्रदान करता है।"
type: docs
weight: 24
url: /hi/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

रिवर्स इमेज सर्च ऑपरेशन के लिए विकल्प प्रदान करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | ImageSearchOptions क्लास का एक नया उदाहरण आरंभ करता है। |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | ImageSearchOptions क्लास का एक नया उदाहरण आरंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | इमेज हैश में असंगत बिट्स की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | इमेज हैश में असंगत बिट्स की अधिकतम संख्या सेट करता है। |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | इमेज रिवर्स सर्च अनुरोध के लिए पाए गए इमेज की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | इमेज रिवर्स सर्च अनुरोध के लिए पाए गए इमेज की अधिकतम संख्या सेट करता है। |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | सर्च दस्तावेज़ फ़िल्टर प्राप्त करता है। |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | सर्च दस्तावेज़ फ़िल्टर प्राप्त करता है या सेट करता है। |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


ImageSearchOptions क्लास का एक नया उदाहरण आरंभ करता है।


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


ImageSearchOptions क्लास का एक नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


इमेज हैश में असंगत बिट्स की अधिकतम संख्या प्राप्त करता है। डिफ़ॉल्ट मान 5 है।


**Returns:**
int - छवि हैश में असंगत बिट्स की अधिकतम संख्या।

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


छवि हैश में असंगत बिट्स की अधिकतम संख्या सेट करता है। डिफ़ॉल्ट मान 5 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | छवि हैश में असंगत बिट्स की अधिकतम संख्या। |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


एक इमेज रिवर्स सर्च अनुरोध के लिए पाए गए चित्रों की अधिकतम संख्या प्राप्त करता है। डिफ़ॉल्ट मान 1000 है।


**Returns:**
int - एक इमेज रिवर्स सर्च अनुरोध के लिए पाए गए चित्रों की अधिकतम संख्या।

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


एक इमेज रिवर्स सर्च अनुरोध के लिए पाए गए चित्रों की अधिकतम संख्या सेट करता है। डिफ़ॉल्ट मान 1000 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | एक इमेज रिवर्स सर्च अनुरोध के लिए पाए गए चित्रों की अधिकतम संख्या। |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


सर्च डॉक्यूमेंट फ़िल्टर प्राप्त करता है। SearchDocumentFilter समावेशन लॉजिक पर काम करता है। GroupDocs.Search.Options.SearchDocumentFilter क्लास का उपयोग सर्च डॉक्यूमेंट फ़िल्टर इंस्टेंस बनाने के लिए करें। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि सभी पाए गए दस्तावेज़ लौटाए जाएंगे।


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


सर्च डॉक्यूमेंट फ़िल्टर प्राप्त करता है या सेट करता है। SearchDocumentFilter समावेशन लॉजिक पर काम करता है। GroupDocs.Search.Options.SearchDocumentFilter क्लास का उपयोग सर्च डॉक्यूमेंट फ़िल्टर इंस्टेंस बनाने के लिए करें। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि सभी पाए गए दस्तावेज़ लौटाए जाएंगे।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | सर्च डॉक्यूमेंट फ़िल्टर। |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
