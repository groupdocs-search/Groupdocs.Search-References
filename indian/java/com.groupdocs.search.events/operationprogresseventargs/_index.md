---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "अनुक्रमण ऑपरेशन की प्रगति अपडेट होने की घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

अनुक्रमण ऑपरेशन की प्रगति अपडेट होने की घटना के लिए तर्क दर्शाता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | प्रोसेसिंग के लिए कुल दस्तावेज़ों की संख्या प्राप्त करता है। |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | सफलतापूर्वक प्रोसेस किए गए दस्तावेज़ों की संख्या प्राप्त करता है। |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | छोड़े गए दस्तावेज़ों की संख्या प्राप्त करता है। |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | प्रगति का प्रतिशत प्राप्त करता है। |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | अंतिम प्रोसेस किए गए दस्तावेज़ की कुंजी प्राप्त करता है। |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | अंतिम प्रोसेस किए गए दस्तावेज़ का पाथ प्राप्त करता है। |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | अंतिम प्रोसेस किए गए दस्तावेज़ की स्थिति प्राप्त करता है। |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


प्रोसेसिंग के लिए कुल दस्तावेज़ों की संख्या प्राप्त करता है।


**Returns:**
int - प्रोसेसिंग के लिए कुल दस्तावेज़ों की संख्या।

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


सफलतापूर्वक प्रोसेस किए गए दस्तावेज़ों की संख्या प्राप्त करता है।


**Returns:**
int - सफलतापूर्वक प्रोसेस किए गए दस्तावेज़ों की संख्या।

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


छोड़े गए दस्तावेज़ों की संख्या प्राप्त करता है।


**Returns:**
int - छोड़े गए दस्तावेज़ों की संख्या।

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


प्रगति का प्रतिशत प्राप्त करता है।


**Returns:**
double - प्रगति का प्रतिशत।

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


अंतिम प्रोसेस किए गए दस्तावेज़ की कुंजी प्राप्त करता है।


**Returns:**
java.lang.String - अंतिम प्रोसेस किए गए दस्तावेज़ की कुंजी।

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


अंतिम प्रोसेस किए गए दस्तावेज़ का पाथ प्राप्त करता है।


**Returns:**
java.lang.String - अंतिम प्रोसेस किए गए दस्तावेज़ का पाथ।

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


अंतिम प्रोसेस किए गए दस्तावेज़ की स्थिति प्राप्त करता है।


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

