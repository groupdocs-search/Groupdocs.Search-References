---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज नेटवर्क के एक नोड में त्रुटि उत्पन्न होने की घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

खोज नेटवर्क के एक नोड में त्रुटि उत्पन्न होने की घटना के लिए तर्क दर्शाता है।

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | सर्च नेटवर्क नोड का इंडेक्स प्राप्त करता है। |
|
|  | [getServiceIndex()](#getServiceIndex--) | सर्च नेटवर्क नोड सेवा का इंडेक्स प्राप्त करता है। |
|
|  | [getMessage()](#getMessage--) | त्रुटि संदेश प्राप्त करता है। |
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

### getMessage() {#getMessage--}
```
public final String getMessage()
```


त्रुटि संदेश प्राप्त करता है।


**Returns:**
java.lang.String - त्रुटि संदेश।

