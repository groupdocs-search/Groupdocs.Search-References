---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search for Java API Reference"
description: "फ़ज़ी सर्च एल्गोरिदम के लिए बेस क्लास को दर्शाता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

फ़ज़ी सर्च एल्गोरिदम के लिए बेस क्लास को दर्शाता है।


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | निर्दिष्ट शब्द लंबाई के लिए समानता स्तर प्राप्त करता है। |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | निर्दिष्ट शब्द लंबाई के लिए अधिकतम अनुमत त्रुटियों की संख्या प्राप्त करता है। |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
```


निर्दिष्ट शब्द लंबाई के लिए समानता स्तर प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | termLength | int | शब्द की लंबाई। |
|

**Returns:**
double - समानता स्तर।

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public abstract int getMaxMistakeCount(int termLength)
```


निर्दिष्ट शब्द लंबाई के लिए अधिकतम अनुमत त्रुटियों की संख्या प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | termLength | int | शब्द की लंबाई। |
|

**Returns:**
int - अधिकतम अनुमत त्रुटियों की संख्या।

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
