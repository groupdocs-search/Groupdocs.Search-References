---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "अनुक्रमण ऑपरेशन की प्रगति अपडेट होने की घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 19
url: /hi/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

अनुक्रमण ऑपरेशन की प्रगति अपडेट होने की घटना के लिए तर्क दर्शाता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | प्रोसेसिंग के लिए कुल सेगमेंट्स की संख्या प्राप्त करता है। |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | प्रोसेस्ड सेगमेंट्स की संख्या प्राप्त करता है। |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | प्रगति का प्रतिशत प्राप्त करता है। |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


प्रोसेसिंग के लिए कुल सेगमेंट्स की संख्या प्राप्त करता है।


**Returns:**
int - प्रोसेसिंग के लिए कुल खंडों की संख्या।

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


प्रोसेस्ड सेगमेंट्स की संख्या प्राप्त करता है।


**Returns:**
int - प्रोसेस किए गए खंडों की संख्या।

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


प्रगति का प्रतिशत प्राप्त करता है।


**Returns:**
double - प्रगति का प्रतिशत।

