---
title: "SimilarityLevel"
second_title: "GroupDocs.Search for Java API Reference"
description: "फ़ज़ी सर्च का वह एल्गोरिद्म दर्शाता है जो समानता स्तर निर्दिष्ट करता है।"
type: docs
weight: 35
url: /hi/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

फ़ज़ी खोज का वह एल्गोरिद्म दर्शाता है जो समानता स्तर निर्दिष्ट करता है। समानता स्तर एल्गोरिद्म शब्द की लंबाई के व्युत्क्रमानुपाती अधिकतम त्रुटियों की संख्या की गणना करता है।


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में एक इंडेक्स बना रहा है
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // फज़ी खोज को सक्षम करना
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // फ़ज़ी खोज एल्गोरिद्म बना रहा है
// यह फ़ंक्शन 1 से 4 अक्षर वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या 0 निर्दिष्ट करता है।
// यह 5 से 9 अक्षर वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या 1 निर्दिष्ट करता है।
// यह 10 से 14 अक्षर वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या 2 निर्दिष्ट करता है। और इसी प्रकार।
SearchResult result = index.search(query, options); // इंडेक्स में खोजें
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | SimilarityLevel क्लास का एक नया इंस्टेंस प्रारंभ करता है। |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | SimilarityLevel क्लास का एक नया इंस्टेंस प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | निर्दिष्ट शब्द लंबाई के लिए समानता स्तर मान प्राप्त करता है। |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | निर्दिष्ट शब्द लंबाई के लिए अधिकतम अनुमत त्रुटियों की संख्या प्राप्त करता है। |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


SimilarityLevel क्लास का एक नया इंस्टेंस प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | double | समानता स्तर मान। |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


SimilarityLevel क्लास का एक नया इंस्टेंस प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


निर्दिष्ट शब्द लंबाई के लिए समानता स्तर मान प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | termLength | int | शब्द की लंबाई। |
|

**Returns:**
double - समानता स्तर मान।

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


निर्दिष्ट शब्द लंबाई के लिए अधिकतम अनुमत त्रुटियों की संख्या प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | termLength | int | शब्द की लंबाई। |
|

**Returns:**
int - अधिकतम अनुमत त्रुटियों की संख्या।

