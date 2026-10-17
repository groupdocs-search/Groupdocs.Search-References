---
title: "IndexErrorEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث حدوث خطأ في الفهرس."
type: docs
weight: 16
url: /ar/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

يمثل المعلمات لحدث حدوث خطأ في الفهرس.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getMessage()](#getMessage--) | يحصل على رسالة الخطأ. |
|
|  | [isCritical()](#isCritical--) | يحصل على علم يشير إلى أن الخطأ حدث وهو حرج ويجب إعادة تشغيل الفهرس. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


يحصل على رسالة الخطأ.


**Returns:**
java.lang.String - رسالة الخطأ.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


يحصل على علم يشير إلى أن الخطأ حدث وهو حرج ويجب إعادة تشغيل الفهرس.


**Returns:**
boolean - العلم الذي يشير إلى أن الخطأ حدث وهو حرج ويجب إعادة تشغيل الفهرس.

