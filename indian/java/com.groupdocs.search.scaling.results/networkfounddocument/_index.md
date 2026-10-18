---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search for Java API Reference"
description: "सर्च नेटवर्क में पाया गया दस्तावेज़ का प्रतिनिधित्व करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

सर्च नेटवर्क में पाया गया दस्तावेज़ का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | पाए गए दस्तावेज़ को प्राप्त करता है। |
|
|  | [getShardIndex()](#getShardIndex--) | शार्ड इंडेक्स प्राप्त करता है। |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


पाए गए दस्तावेज़ को प्राप्त करता है।


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


शार्ड इंडेक्स प्राप्त करता है।


**Returns:**
int - शार्ड इंडेक्स।

