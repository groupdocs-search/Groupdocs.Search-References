---
title: "HighlightOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "पाए गए शब्दों को हाइलाइट करने के लिए विकल्प प्रदान करता है।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

पाए गए शब्दों को हाइलाइट करने के लिए विकल्प प्रदान करता है।


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) |   HighlightOptions  क्लास का एक नया उदाहरण आरंभ करता है। |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) |   TextOptions  क्लास का एक नया उदाहरण आरंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | हाइलाइट किए गए शब्द से पहले टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | हाइलाइट किए गए शब्द से पहले टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या सेट करता है। |
|
|  | [getTermsAfter()](#getTermsAfter--) | हाइलाइट किए गए शब्द के बाद टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | हाइलाइट किए गए शब्द के बाद टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या सेट करता है। |
|
|  | [getTermsTotal()](#getTermsTotal--) | टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या सेट करता है। |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | एक मान प्राप्त करता है जो दर्शाता है कि क्या इनलाइन स्टाइल्स का उपयोग घटनाओं को हाइलाइट करने के लिए किया जाता है। |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | एक मान सेट करता है जो दर्शाता है कि क्या इनलाइन स्टाइल्स का उपयोग घटनाओं को हाइलाइट करने के लिए किया जाता है। |
|
|  | [getHighlightColor()](#getHighlightColor--) | एक रंग प्राप्त करता है जो घटनाओं को हाइलाइट करने के लिए उपयोग किया जाता है। |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | एक रंग सेट करता है जिसका उपयोग घटनाओं को उजागर करने के लिए किया जाता है। |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | पाए गए शब्द के हाइलाइट करने के प्रारंभ टैग को प्राप्त करता है। |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | पाए गए शब्द के हाइलाइट करने के प्रारंभ टैग को सेट करता है। |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | पाए गए शब्द के हाइलाइट करने के समाप्ति टैग को प्राप्त करता है। |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | पाए गए शब्द के हाइलाइट करने के समाप्ति टैग को सेट करता है। |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


  HighlightOptions  क्लास का एक नया उदाहरण आरंभ करता है।


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


  TextOptions  क्लास का एक नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


हाइलाइट किए गए शब्द से पहले टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या प्राप्त करता है। मान 0 से 10000 की सीमा में होना चाहिए। डिफ़ॉल्ट मान 7 है।


**Returns:**
int - हाइलाइट किए गए शब्द से पहले टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या।

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


हाइलाइट किए गए शब्द से पहले टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या सेट करता है। मान 0 से 10000 की सीमा में होना चाहिए। डिफ़ॉल्ट मान 7 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | हाइलाइट किए गए शब्द से पहले टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या। |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


हाइलाइट किए गए शब्द के बाद टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या प्राप्त करता है। मान 0 से 10000 की सीमा में होना चाहिए। डिफ़ॉल्ट मान 7 है।


**Returns:**
int - हाइलाइट किए गए शब्द के बाद टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या।

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


हाइलाइट किए गए शब्द के बाद टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या सेट करता है। मान 0 से 10000 की सीमा में होना चाहिए। डिफ़ॉल्ट मान 7 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | हाइलाइट किए गए शब्द के बाद टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या। |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या प्राप्त करता है। मान 0 से 10000 की सीमा में होना चाहिए। डिफ़ॉल्ट मान 21 है।


**Returns:**
int - टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या।

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या सेट करता है। मान 0 से 10000 की सीमा में होना चाहिए। डिफ़ॉल्ट मान 21 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | टेक्स्ट स्निपेट में शब्दों की अधिकतम संख्या। |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


हाइलाइट किए गए घटनाओं के लिए इनलाइन स्टाइल्स का उपयोग किया जाता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। डिफ़ॉल्ट मान true है।


**Returns:**
boolean - हाइलाइट किए गए घटनाओं के लिए इनलाइन स्टाइल्स का उपयोग किया जाता है या नहीं, यह दर्शाने वाला मान।

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


हाइलाइट किए गए घटनाओं के लिए इनलाइन स्टाइल्स का उपयोग किया जाता है या नहीं, यह दर्शाने वाला मान सेट करता है। डिफ़ॉल्ट मान true है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | हाइलाइट किए गए घटनाओं के लिए इनलाइन स्टाइल्स का उपयोग किया जाता है या नहीं, यह दर्शाने वाला मान। |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


हाइलाइट किए गए घटनाओं के लिए उपयोग किया जाने वाला रंग प्राप्त करता है। डिफ़ॉल्ट मान #FFD800 है।


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


हाइलाइट किए गए घटनाओं के लिए उपयोग किया जाने वाला रंग सेट करता है। डिफ़ॉल्ट मान #FFD800 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | एक रंग जो घटनाओं को उजागर करने के लिए उपयोग किया जाता है। |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


पाए गए शब्द को उजागर करने के प्रारंभ टैग को प्राप्त करता है। यह टैग केवल साधारण पाठ में उजागर करने पर उपयोग किया जाता है। डिफ़ॉल्ट मान एक खाली स्ट्रिंग है।


**Returns:**
java.lang.String - पाए गए शब्द को उजागर करने के प्रारंभ टैग।

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


पाए गए शब्द को उजागर करने के प्रारंभ टैग को सेट करता है। यह टैग केवल साधारण पाठ में उजागर करने पर उपयोग किया जाता है। डिफ़ॉल्ट मान एक खाली स्ट्रिंग है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | पाए गए शब्द को उजागर करने का प्रारंभ टैग। |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


पाए गए शब्द को उजागर करने के समाप्ति टैग को प्राप्त करता है। यह टैग केवल साधारण पाठ में उजागर करने पर उपयोग किया जाता है। डिफ़ॉल्ट मान एक खाली स्ट्रिंग है।


**Returns:**
java.lang.String - पाए गए शब्द को उजागर करने का समाप्ति टैग।

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


पाए गए शब्द को उजागर करने के समाप्ति टैग को सेट करता है। यह टैग केवल साधारण पाठ में उजागर करने पर उपयोग किया जाता है। डिफ़ॉल्ट मान एक खाली स्ट्रिंग है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | पाए गए शब्द को उजागर करने का समाप्ति टैग। |
|

