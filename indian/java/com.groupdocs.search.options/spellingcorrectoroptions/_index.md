---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "स्पेलिंग करेक्टर के लिए विकल्प प्रदान करता है।"
type: docs
weight: 36
url: /hi/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

स्पेलिंग करेक्टर के लिए विकल्प प्रदान करता है।


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | एक मान प्राप्त करता है जो दर्शाता है कि वर्तनी सुधारक सक्षम है या नहीं। |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | एक मान सेट करता है जो दर्शाता है कि वर्तनी सुधारक सक्षम है या नहीं। |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | त्रुटियों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | त्रुटियों की अधिकतम संख्या सेट करता है। |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | एक मान प्राप्त करता है जो दर्शाता है कि केवल सर्वोत्तम परिणाम लौटाए जाएंगे या नहीं। |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | एक मान सेट करता है जो दर्शाता है कि केवल सर्वोत्तम परिणाम लौटाए जाएंगे या नहीं। |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | पाए गए न्यूनतम त्रुटियों की संख्या से अधिकतम अधिकता प्राप्त करता है। |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | पाए गए न्यूनतम त्रुटियों की संख्या से अधिकतम अधिकता सेट करता है। |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | एक मान प्राप्त करता है जो दर्शाता है कि एल्गोरिद्म को दो सटे हुए अक्षरों के स्थानांतरण को एक ही त्रुटि के रूप में मानना चाहिए या नहीं। |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | एक मान सेट करता है जो दर्शाता है कि एल्गोरिद्म को दो सटे हुए अक्षरों के स्थानांतरण को एक ही त्रुटि के रूप में मानना चाहिए या नहीं। |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


एक मान प्राप्त करता है जो दर्शाता है कि वर्तनी सुधारक सक्षम है या नहीं। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - एक मान जो दर्शाता है कि वर्तनी सुधारक सक्षम है या नहीं।

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि वर्तनी सुधारक सक्षम है या नहीं। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | एक मान जो दर्शाता है कि वर्तनी सुधारक सक्षम है या नहीं। |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


त्रुटियों की अधिकतम संख्या प्राप्त करता है। डिफ़ॉल्ट मान 2 है।


**Returns:**
int - अधिकतम त्रुटियों की संख्या।

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


अधिकतम त्रुटियों की संख्या सेट करता है। डिफ़ॉल्ट मान  2  है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | अधिकतम त्रुटियों की संख्या। |
|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि केवल सर्वोत्तम परिणाम लौटाए जाएंगे या नहीं। डिफ़ॉल्ट मान  false  है।


**Returns:**
boolean -  true  यदि केवल सर्वोत्तम परिणाम लौटाए जाएंगे; अन्यथा  false .

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि केवल सर्वोत्तम परिणाम लौटाए जाएंगे या नहीं। डिफ़ॉल्ट मान  false  है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | true  यदि केवल सर्वोत्तम परिणाम लौटाए जाएंगे; अन्यथा  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


पाए गए न्यूनतम त्रुटियों की संख्या से अधिकतम अधिकता प्राप्त करता है। डिफ़ॉल्ट मान  0  है।


**Returns:**
byte - पाए गए न्यूनतम त्रुटियों की संख्या से अधिकतम अधिकता।

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


पाए गए न्यूनतम त्रुटियों की संख्या से अधिकतम अधिकता सेट करता है। डिफ़ॉल्ट मान  0  है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | byte | पाए गए न्यूनतम त्रुटियों की संख्या से अधिकतम अधिकता। |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि एल्गोरिद्म को दो क्रमागत अक्षरों के स्थानांतरण को एक ही त्रुटि के रूप में विचार करना चाहिए या नहीं। डिफ़ॉल्ट मान  true  है।


**Returns:**
boolean -  true  यदि वर्तनी सुधारक एल्गोरिद्म स्थानांतरण को मानता है; अन्यथा  false .

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


एक मान सेट करता है जो यह दर्शाता है कि एल्गोरिद्म को दो क्रमागत अक्षरों के स्थानांतरण को एक ही त्रुटि के रूप में विचार करना चाहिए या नहीं। डिफ़ॉल्ट मान  true  है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | true  यदि वर्तनी सुधारक एल्गोरिद्म स्थानांतरण को मानता है; अन्यथा  false . |
|

