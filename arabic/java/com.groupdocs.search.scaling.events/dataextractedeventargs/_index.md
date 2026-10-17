---
title: "DataExtractedEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث انتهاء استخراج بيانات المستند."
type: docs
weight: 10
url: /ar/java/com.groupdocs.search.scaling.events/dataextractedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DataExtractedEventArgs extends EventArgs
```

يمثل المعلمات لحدث انتهاء استخراج بيانات المستند.

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getExtractorIndex()](#getExtractorIndex--) | يحصل على فهرس المستخرج. |
|
|  | [getDocumentKey()](#getDocumentKey--) | يحصل على مفتاح المستند. |
|
### getExtractorIndex() {#getExtractorIndex--}
```
public final int getExtractorIndex()
```


يحصل على فهرس المستخرج.


**Returns:**
int - فهرس المستخرج.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


يحصل على مفتاح المستند.


**Returns:**
java.lang.String - مفتاح المستند.

