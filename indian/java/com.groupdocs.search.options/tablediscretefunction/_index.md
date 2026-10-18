---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search for Java API Reference"
description: "फ़ज़ी सर्च एल्गोरिद्म को दर्शाता है जिसमें शब्द लंबाई और अनुमत त्रुटियों की संख्या के बीच संबंध होते हैं।"
type: docs
weight: 40
url: /hi/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

फ़ज़ी खोज एल्गोरिदम का प्रतिनिधित्व करता है जिसमें शब्द लंबाई और अनुमत त्रुटियों की संख्या के बीच संबंध होते हैं। इस एल्गोरिदम को आउटपुट मानों की तालिका या चरण फ़ंक्शन द्वारा निर्दिष्ट किया जा सकता है।


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // फ़ज़ी खोज एल्गोरिदम बना रहा है
// यह फ़ंक्शन 1 को 1 से 4 अक्षरों वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या के रूप में निर्दिष्ट करता है।
// यह 5 से 7 अक्षरों वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या के रूप में 2 को निर्दिष्ट करता है।
// यह 8 या अधिक अक्षरों वाले शब्दों के लिए अधिकतम त्रुटियों की संख्या के रूप में 3 को निर्दिष्ट करता है।
SearchResult result = index.search(query, options); // इंडेक्स में खोजें
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | TableDiscreteFunction क्लास का एक नया उदाहरण आरंभ करता है। |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | TableDiscreteFunction क्लास का एक नया उदाहरण आरंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | निर्दिष्ट शब्द लंबाई के लिए समानता स्तर प्राप्त करता है। |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | निर्दिष्ट शब्द लंबाई के लिए अनुमत अधिकतम त्रुटियों की संख्या प्राप्त करता है। |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


TableDiscreteFunction क्लास का एक नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | offsetOfInputs | int | इनपुट मानों के सापेक्ष तालिका इंडेक्स का ऑफ़सेट। |
|
|  | tableOfOutputs | int[] | आउटपुट मानों की तालिका। |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


TableDiscreteFunction क्लास का एक नया उदाहरण आरंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | firstStepLevel | int | स्टेप फ़ंक्शन के पहले चरण का स्तर। |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | स्टेप फ़ंक्शन के अगले चरण। |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


निर्दिष्ट शब्द लंबाई के लिए समानता स्तर प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | termLength | int | शब्द की लंबाई। |
|

**Returns:**
double - एक समानता स्तर।

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


निर्दिष्ट शब्द लंबाई के लिए अनुमत अधिकतम त्रुटियों की संख्या प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | termLength | int | शब्द की लंबाई। |
|

**Returns:**
int - अनुमत अधिकतम त्रुटियों की संख्या।

