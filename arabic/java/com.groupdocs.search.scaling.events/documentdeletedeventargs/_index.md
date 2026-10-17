---
title: "DocumentDeletedEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث انتهاء حذف المستند."
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.scaling.events/documentdeletedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentDeletedEventArgs extends EventArgs
```

يمثل المعلمات لحدث انتهاء حذف المستند.

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | يحصل على فهرس الجزء. |
|
|  | [getDocumentKey()](#getDocumentKey--) | يحصل على مفتاح المستند. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


يحصل على فهرس الجزء.


**Returns:**
int - فهرس الجزء.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


يحصل على مفتاح المستند.


**Returns:**
java.lang.String - مفتاح المستند.

