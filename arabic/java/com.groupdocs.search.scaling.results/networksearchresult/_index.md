---
title: "NetworkSearchResult"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نتيجة بحث تتطابق مع استعلام البحث."
type: docs
weight: 14
url: /ar/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

يمثل نتيجة بحث تتطابق مع استعلام البحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | يحصل على عدد المستندات التي تم العثور عليها. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | يحصل على إجمالي عدد التكرارات التي تم العثور عليها. |
|
|  | [getTruncated()](#getTruncated--) | يحصل على قيمة تشير إلى أن النتيجة مقطوعة. |
|
|  | [getWarnings()](#getWarnings--) | يحصل على تحذير يصف النتيجة. |
|
|  | [getStartTime()](#getStartTime--) | يحصل على وقت بدء البحث. |
|
|  | [getEndTime()](#getEndTime--) | يحصل على وقت انتهاء البحث. |
|
|  | [getSearchDuration()](#getSearchDuration--) | يحصل على مدة البحث بالثواني. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | يحصل على المستند الموجود حسب الفهرس. |
|
|  | [iterator()](#iterator--) | يرجع مُكرِّرًا يتنقل عبر مجموعة المستندات التي تم العثور عليها. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | يحصل على رمز بحث القطعة للبحث عن القطعة التالية. |
|
|  | [getNodeIndex()](#getNodeIndex--) | يحصل على فهرس العقدة التي تم استلام النتيجة منها. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


يحصل على عدد المستندات التي تم العثور عليها.


**Returns:**
int - عدد المستندات التي تم العثور عليها.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


يحصل على إجمالي عدد التكرارات التي تم العثور عليها.


**Returns:**
int - إجمالي عدد التكرارات التي تم العثور عليها.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


يحصل على قيمة تشير إلى أن النتيجة مقطوعة.


**Returns:**
boolean - قيمة تشير إلى أن النتيجة مقطوعة.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


يحصل على تحذير يصف النتيجة.


**Returns:**
java.lang.String - تحذير يصف النتيجة.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


يحصل على وقت بدء البحث.


**Returns:**
java.util.Date - وقت بدء البحث.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


يحصل على وقت انتهاء البحث.


**Returns:**
java.util.Date - وقت انتهاء البحث.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


يحصل على مدة البحث بالثواني.


**Returns:**
double - مدة البحث بالثواني.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


يحصل على المستند الموجود حسب الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | الفهرس | int | فهرس المستند الذي تم العثور عليه. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


يرجع مُكرِّرًا يتنقل عبر مجموعة المستندات التي تم العثور عليها.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - مكرِّر يمكن استخدامه للتنقل عبر مجموعة المستندات التي تم العثور عليها.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


يحصل على رمز بحث القطعة للبحث عن القطعة التالية.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


يحصل على فهرس العقدة التي تم استلام النتيجة منها.


**Returns:**
int - فهرس العقدة التي تم استلام النتيجة منها.

