---
title: "NetworkImageSearchResult"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نتيجة بحث صورة تتطابق مع صورة البحث."
type: docs
weight: 12
url: /ar/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

يمثل نتيجة بحث صورة تتطابق مع صورة البحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | يحصل على عدد الصور التي تم العثور عليها. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | يحصل على الصورة الموجودة حسب الفهرس. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | يحصل على رمز بحث صورة مقطع للبحث عن المقطع التالي. |
|
|  | [getNodeIndex()](#getNodeIndex--) | يحصل على فهرس العقدة التي تم استلام النتيجة منها. |
|
|  | [getShardIndex()](#getShardIndex--) | يحصل على فهرس الـshard الذي تم استلام النتيجة منه. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


يحصل على عدد الصور التي تم العثور عليها.


**Returns:**
int - عدد الصور التي تم العثور عليها.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


يحصل على الصورة الموجودة حسب الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | الفهرس | int | فهرس الصورة التي تم العثور عليها. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


يحصل على رمز بحث صورة مقطع للبحث عن المقطع التالي.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


يحصل على فهرس العقدة التي تم استلام النتيجة منها.


**Returns:**
int - فهرس العقدة التي تم استلام النتيجة منها.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


يحصل على فهرس الـshard الذي تم استلام النتيجة منه.


**Returns:**
int - فهرس الـshard الذي تم استلام النتيجة منه.

