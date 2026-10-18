---
title: "DeleteResult"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स से इंडेक्स्ड फ़ाइलों या फ़ोल्डरों को हटाने के ऑपरेशन के परिणाम का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

इंडेक्स से इंडेक्स्ड फ़ाइलों या फ़ोल्डरों को हटाने के ऑपरेशन के परिणाम का प्रतिनिधित्व करता है।


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | प्रत्येक पाथ को हटाने के परिणाम लौटाता है। |
|
|  | [getTotalCount()](#getTotalCount--) | हटाने के लिए पाथ की कुल संख्या लौटाता है। |
|
|  | [getSuccessCount()](#getSuccessCount--) | सफलतापूर्वक हटाए गए पाथ की संख्या लौटाता है। |
|
|  | [getFailedCount()](#getFailedCount--) | त्रुटियों के कारण न हटाए गए पाथ की संख्या लौटाता है। |
|
|  | [getErrors()](#getErrors--) | हटाने की त्रुटियों का विवरण लौटाता है। |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


प्रत्येक पाथ को हटाने के परिणाम लौटाता है।


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - प्रत्येक पाथ को हटाने के परिणाम।

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


हटाने के लिए पाथ की कुल संख्या लौटाता है।


**Returns:**
int - हटाने के लिए पाथ की कुल संख्या।

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


सफलतापूर्वक हटाए गए पाथ की संख्या लौटाता है।


**Returns:**
int - सफलतापूर्वक हटाए गए पथों की संख्या।

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


त्रुटियों के कारण न हटाए गए पाथ की संख्या लौटाता है।


**Returns:**
int - त्रुटियों के कारण न हटाए गए पथों की संख्या।

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


हटाने की त्रुटियों का विवरण लौटाता है।


**Returns:**
java.lang.String[] - हटाने की त्रुटियों के विवरण।

