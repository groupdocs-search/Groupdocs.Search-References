---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक खोज छवि से मेल खाने वाले इमेज सर्च परिणाम का प्रतिनिधित्व करता है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

एक खोज छवि से मेल खाने वाले इमेज सर्च परिणाम का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | पाए गए चित्रों की संख्या प्राप्त करता है। |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | सूचकांक द्वारा पाए गए चित्र को प्राप्त करता है। |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | अगले भाग की खोज के लिए एक चंक इमेज सर्च टोकन प्राप्त करता है। |
|
|  | [getNodeIndex()](#getNodeIndex--) | जिस नोड से परिणाम प्राप्त हुआ, उसका सूचकांक प्राप्त करता है। |
|
|  | [getShardIndex()](#getShardIndex--) | जिस शार्ड से परिणाम प्राप्त हुआ, उसका सूचकांक प्राप्त करता है। |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


पाए गए चित्रों की संख्या प्राप्त करता है।


**Returns:**
int - पाए गए चित्रों की संख्या।

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


सूचकांक द्वारा पाए गए चित्र को प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इंडेक्स | int | पाए गए चित्र का सूचकांक। |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


अगले भाग की खोज के लिए एक चंक इमेज सर्च टोकन प्राप्त करता है।


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


जिस नोड से परिणाम प्राप्त हुआ, उसका सूचकांक प्राप्त करता है।


**Returns:**
int - जिस नोड से परिणाम प्राप्त हुआ, उसका सूचकांक।

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


जिस शार्ड से परिणाम प्राप्त हुआ, उसका सूचकांक प्राप्त करता है।


**Returns:**
int - जिस शार्ड से परिणाम प्राप्त हुआ, उसका सूचकांक।

