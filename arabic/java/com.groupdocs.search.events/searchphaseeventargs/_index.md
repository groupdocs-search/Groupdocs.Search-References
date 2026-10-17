---
title: "SearchPhaseEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لأحداث تغيير مرحلة البحث."
type: docs
weight: 21
url: /ar/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

يمثل المعلمات لأحداث تغيير مرحلة البحث.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | يحصل على مرحلة البحث. |
|
|  | [getQuery()](#getQuery--) | يحصل على الاستعلام الأولي للبحث الحالي. |
|
|  | [getWords()](#getWords--) | يحصل على الكلمات التي تم الحصول عليها في المرحلة الحالية. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


يحصل على مرحلة البحث.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


يحصل على الاستعلام الأولي للبحث الحالي.


**Returns:**
java.lang.String - الاستعلام الأولي للبحث الحالي.

### getWords() {#getWords--}
```
public final String[] getWords()
```


يحصل على الكلمات التي تم الحصول عليها في المرحلة الحالية.


**Returns:**
java.lang.String[] - الكلمات التي تم الحصول عليها في المرحلة الحالية.

