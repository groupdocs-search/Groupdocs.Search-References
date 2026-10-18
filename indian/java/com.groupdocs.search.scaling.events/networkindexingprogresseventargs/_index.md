---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "अनुक्रमण ऑपरेशन की प्रगति परिवर्तन घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

अनुक्रमण ऑपरेशन की प्रगति परिवर्तन घटना के लिए तर्क दर्शाता है।

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | सर्च नेटवर्क नोड का इंडेक्स प्राप्त करता है। |
|
|  | [getServiceIndex()](#getServiceIndex--) | सर्च नेटवर्क नोड सेवा का इंडेक्स प्राप्त करता है। |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | प्रोसेस किए गए दस्तावेज़ों की संख्या प्राप्त करता है। |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | प्रोसेसिंग के लिए कुल दस्तावेज़ों की संख्या प्राप्त करता है। |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | प्रगति का प्रतिशत प्राप्त करता है। |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


सर्च नेटवर्क नोड का इंडेक्स प्राप्त करता है।


**Returns:**
int - सर्च नेटवर्क नोड का इंडेक्स।

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


सर्च नेटवर्क नोड सेवा का इंडेक्स प्राप्त करता है।


**Returns:**
int - सर्च नेटवर्क नोड सेवा का इंडेक्स।

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


प्रोसेस किए गए दस्तावेज़ों की संख्या प्राप्त करता है।


**Returns:**
int - प्रोसेस किए गए दस्तावेज़ों की संख्या।

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


प्रोसेसिंग के लिए कुल दस्तावेज़ों की संख्या प्राप्त करता है।


**Returns:**
int - प्रोसेसिंग के लिए कुल दस्तावेज़ों की संख्या।

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


प्रगति का प्रतिशत प्राप्त करता है।


**Returns:**
double - प्रगति का प्रतिशत।

