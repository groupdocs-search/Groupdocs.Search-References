---
title: "IndexInfo"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحتوي على معلومات أساسية حول الفهرس."
type: docs
weight: 24
url: /ar/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

يحتوي على معلومات أساسية عن الفهرس.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | يحصل على المعرف الفريد للفهرس. |
|
|  | [getIndexFolder()](#getIndexFolder--) | يحصل على اسم المجلد الكامل حيث يقع الفهرس. |
|
|  | [getIndexStatus()](#getIndexStatus--) | يحصل على حالة الفهرس. |
|
|  | [getVersion()](#getVersion--) | يحصل على نسخة الفهرس. |
|
|  | [getSegmentCount()](#getSegmentCount--) | يحصل على عدد مقاطع الفهرس. |
|
|  | [getTermCount()](#getTermCount--) | يسترجع عدد الكلمات في الفهرس. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


يحصل على المعرف الفريد للفهرس.


**Returns:**
java.util.UUID - المعرف الفريد للفهرس.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


يحصل على اسم المجلد الكامل حيث يقع الفهرس.


**Returns:**
java.lang.String - الاسم الكامل للمجلد الذي يقع فيه الفهرس.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


يحصل على حالة الفهرس.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


يحصل على نسخة الفهرس.


**Returns:**
java.lang.String - إصدار الفهرس.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


يحصل على عدد مقاطع الفهرس.


**Returns:**
int - عدد مقاطع الفهرس.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


يسترجع عدد الكلمات في الفهرس.


**Returns:**
int - عدد الكلمات في الفهرس.

