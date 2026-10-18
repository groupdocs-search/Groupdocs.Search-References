---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक खोज क्वेरी से मेल खाने वाले सर्च परिणाम का प्रतिनिधित्व करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

एक खोज क्वेरी से मेल खाने वाले सर्च परिणाम का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | पाए गए दस्तावेज़ों की संख्या प्राप्त करता है। |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | पाए गए कुल घटनाओं की संख्या प्राप्त करता है। |
|
|  | [getTruncated()](#getTruncated--) | परिणाम के कटे हुए होने को दर्शाने वाला मान प्राप्त करता है। |
|
|  | [getWarnings()](#getWarnings--) | परिणाम का वर्णन करने वाली चेतावनी प्राप्त करता है। |
|
|  | [getStartTime()](#getStartTime--) | खोज की प्रारंभिक समय प्राप्त करता है। |
|
|  | [getEndTime()](#getEndTime--) | खोज का समाप्ति समय प्राप्त करता है। |
|
|  | [getSearchDuration()](#getSearchDuration--) | खोज की अवधि सेकंड में प्राप्त करता है। |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | सूचकांक द्वारा पाए गए दस्तावेज़ को प्राप्त करता है। |
|
|  | [iterator()](#iterator--) | पाए गए दस्तावेज़ों के संग्रह के माध्यम से इटरेट करने वाला इटरेटर लौटाता है। |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | अगले भाग की खोज के लिए एक चंक सर्च टोकन प्राप्त करता है। |
|
|  | [getNodeIndex()](#getNodeIndex--) | जिस नोड से परिणाम प्राप्त हुआ, उसका सूचकांक प्राप्त करता है। |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


पाए गए दस्तावेज़ों की संख्या प्राप्त करता है।


**Returns:**
int - पाए गए दस्तावेज़ों की संख्या।

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


पाए गए कुल घटनाओं की संख्या प्राप्त करता है।


**Returns:**
int - पाए गए कुल घटनाओं की संख्या।

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


परिणाम के कटे हुए होने को दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean - परिणाम के कटे हुए होने को दर्शाने वाला मान।

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


परिणाम का वर्णन करने वाली चेतावनी प्राप्त करता है।


**Returns:**
java.lang.String - परिणाम का वर्णन करने वाली चेतावनी।

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


खोज की प्रारंभिक समय प्राप्त करता है।


**Returns:**
java.util.Date - खोज की प्रारंभिक समय।

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


खोज का समाप्ति समय प्राप्त करता है।


**Returns:**
java.util.Date - खोज का समाप्ति समय।

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


खोज की अवधि सेकंड में प्राप्त करता है।


**Returns:**
double - खोज की अवधि सेकंड में।

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


सूचकांक द्वारा पाए गए दस्तावेज़ को प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इंडेक्स | int | पाए गए दस्तावेज़ का सूचकांक। |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


पाए गए दस्तावेज़ों के संग्रह के माध्यम से इटरेट करने वाला इटरेटर लौटाता है।


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - पाए गए दस्तावेज़ों के संग्रह के माध्यम से इटरेट करने के लिए उपयोग किया जा सकने वाला इटरेटर।

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


अगले भाग की खोज के लिए एक चंक सर्च टोकन प्राप्त करता है।


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


जिस नोड से परिणाम प्राप्त हुआ, उसका सूचकांक प्राप्त करता है।


**Returns:**
int - जिस नोड से परिणाम प्राप्त हुआ, उसका सूचकांक।

