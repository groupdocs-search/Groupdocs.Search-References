---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search for Java API Reference"
description: "सर्च नेटवर्क में इंडेक्स्ड दस्तावेज़ के लिए एक डिस्क्रिप्टर का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

सर्च नेटवर्क में इंडेक्स्ड दस्तावेज़ के लिए एक डिस्क्रिप्टर का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | एक अनुक्रमित दस्तावेज़ के लिए वर्णनकर्ता को प्राप्त करता है। |
|
|  | [getShardIndex()](#getShardIndex--) | शार्ड इंडेक्स प्राप्त करता है। |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


एक अनुक्रमित दस्तावेज़ के लिए वर्णनकर्ता को प्राप्त करता है।


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


शार्ड इंडेक्स प्राप्त करता है।


**Returns:**
int - शार्ड इंडेक्स।

