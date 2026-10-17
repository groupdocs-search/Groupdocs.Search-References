---
title: "BaseIndexEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل الفئة الأساسية لمعلمات الحدث."
type: docs
weight: 10
url: /ar/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

يمثل الفئة الأساسية لمعلمات الحدث.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getTime()](#getTime--) | يحصل على وقت الحدث. |
|
|  | [getIndexId()](#getIndexId--) | يحصل على معرف الفهرس. |
|
|  | [getIndexFolder()](#getIndexFolder--) | يحصل على مجلد الفهرس. |
|
|  | [getStatus()](#getStatus--) | يحصل على حالة الفهرس. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


يحصل على وقت الحدث.


**Returns:**
java.util.Date - وقت الحدث.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


يحصل على معرف الفهرس.


**Returns:**
java.util.UUID - معرف الفهرس.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


يحصل على مجلد الفهرس.


**Returns:**
java.lang.String - مجلد الفهرس.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


يحصل على حالة الفهرس.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

