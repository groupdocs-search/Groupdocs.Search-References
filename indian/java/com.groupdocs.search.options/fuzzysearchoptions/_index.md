---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "फ़ज़ी सर्च के विकल्प प्रदान करता है।"
type: docs
weight: 21
url: /hi/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

फ़ज़ी सर्च के विकल्प प्रदान करता है।


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | फज़ी खोज सुविधा सक्षम है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | फ़ज़ी खोज सुविधा सक्षम है या नहीं, यह दर्शाने वाला मान सेट करता है। |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | फ़ज़ी खोज एल्गोरिद्म प्राप्त करता है। |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | फ़ज़ी खोज एल्गोरिद्म सेट करता है। |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | एक मान प्राप्त करता है जो दर्शाता है कि केवल सर्वोत्तम परिणाम लौटाए जाएंगे या नहीं। |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | एक मान सेट करता है जो दर्शाता है कि केवल सर्वोत्तम परिणाम लौटाए जाएंगे या नहीं। |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | पाए गए न्यूनतम त्रुटियों की संख्या से अधिकतम अधिकता प्राप्त करता है। |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | पाए गए न्यूनतम त्रुटियों की संख्या से अधिकतम अधिकता सेट करता है। |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | फ़ज़ी खोज एल्गोरिद्म को दो सन्निकट अक्षरों के स्थानांतरण को एक ही गलती के रूप में विचार करना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | फ़ज़ी खोज एल्गोरिद्म को दो सन्निकट अक्षरों के स्थानांतरण को एक ही गलती के रूप में विचार करना चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है। |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


फ़ज़ी खोज सुविधा सक्षम है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - फ़ज़ी खोज सुविधा सक्षम है या नहीं, यह दर्शाने वाला मान।

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


फ़ज़ी खोज सुविधा सक्षम है या नहीं, यह दर्शाने वाला मान सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | फ़ज़ी खोज सुविधा सक्षम है या नहीं, यह दर्शाने वाला मान। |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


फ़ज़ी खोज एल्गोरिद्म प्राप्त करता है। वर्तमान में उपलब्ध फ़ज़ी खोज एल्गोरिद्म SimilarityLevel और TableDiscreteFunction हैं। डिफ़ॉल्ट मान SimilarLevel का एक उदाहरण है, जिसका समानता स्तर मान 0.5 है।


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


उदाहरण दर्शाता है कि फ़ज़ी खोज एल्गोरिद्म कैसे सेट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में एक इंडेक्स बना रहा है
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // फज़ी खोज को सक्षम करना
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // फ़ज़ी खोज एल्गोरिदम बना रहा है
// यह फ़ंक्शन 1 को 1 से 4 अक्षरों वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या के रूप में निर्दिष्ट करता है।
// यह 5 से 7 अक्षरों वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या के रूप में 2 को निर्दिष्ट करता है।
// यह 8 या अधिक अक्षरों वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या के रूप में 3 को निर्दिष्ट करता है।
SearchResult result = index.search(query, options); // इंडेक्स में खोजें
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


फ़ज़ी खोज एल्गोरिद्म सेट करता है। वर्तमान में उपलब्ध फ़ज़ी खोज एल्गोरिद्म SimilarityLevel और TableDiscreteFunction हैं। डिफ़ॉल्ट मान SimilarLevel का एक उदाहरण है, जिसका समानता स्तर मान 0.5 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | फ़ज़ी खोज एल्गोरिद्म। |


उदाहरण दर्शाता है कि फ़ज़ी खोज एल्गोरिद्म कैसे सेट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में एक इंडेक्स बना रहा है
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // फज़ी खोज को सक्षम करना
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // फ़ज़ी खोज एल्गोरिदम बना रहा है
// यह फ़ंक्शन 1 को 1 से 4 अक्षरों वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या के रूप में निर्दिष्ट करता है।
// यह 5 से 7 अक्षरों वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या के रूप में 2 को निर्दिष्ट करता है।
// यह 8 या अधिक अक्षरों वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या के रूप में 3 को निर्दिष्ट करता है।
SearchResult result = index.search(query, options); // इंडेक्स में खोजें
 
```
 
````

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


फ़ज़ी खोज एल्गोरिद्म को दो सन्निकट अक्षरों के स्थानांतरण को एक ही गलती के रूप में विचार करना चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है। डिफ़ॉल्ट मान true है।


**Returns:**
boolean - यदि फ़ज़ी खोज एल्गोरिद्म स्थानांतरण को विचार करता है तो true; अन्यथा false।

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


फ़ज़ी खोज एल्गोरिद्म को दो सन्निकट अक्षरों के स्थानांतरण को एक ही गलती के रूप में विचार करना चाहिए या नहीं, यह दर्शाने वाला मान सेट करता है। डिफ़ॉल्ट मान true है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | : true यदि फ़ज़ी खोज एल्गोरिद्म स्थानांतरण को विचार करता है; अन्यथा false। |
|

