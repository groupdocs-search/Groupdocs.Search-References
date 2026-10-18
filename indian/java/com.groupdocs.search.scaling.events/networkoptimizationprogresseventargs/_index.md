---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "अनुकूलन ऑपरेशन की प्रगति परिवर्तन घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

अनुकूलन ऑपरेशन की प्रगति परिवर्तन घटना के लिए तर्क दर्शाता है।

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | सर्च नेटवर्क नोड का इंडेक्स प्राप्त करता है। |
|
|  | [getServiceIndex()](#getServiceIndex--) | सर्च नेटवर्क नोड सेवा का इंडेक्स प्राप्त करता है। |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | प्रोसेस्ड सेगमेंट्स की संख्या प्राप्त करता है। |
|
|  | [getTotalSegments()](#getTotalSegments--) | प्रोसेसिंग के लिए कुल सेगमेंट्स की संख्या प्राप्त करता है। |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


प्रोसेस्ड सेगमेंट्स की संख्या प्राप्त करता है।


**Returns:**
int - प्रोसेस किए गए खंडों की संख्या।

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


प्रोसेसिंग के लिए कुल सेगमेंट्स की संख्या प्राप्त करता है।


**Returns:**
int - प्रोसेसिंग के लिए कुल खंडों की संख्या।

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


प्रगति का प्रतिशत प्राप्त करता है।


**Returns:**
double - प्रगति का प्रतिशत।

