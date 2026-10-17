---
title: "ExtractorSettings"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحتوي على إعدادات مستخرج بيانات المستند."
type: docs
weight: 19
url: /ar/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

يحتوي على إعدادات مستخرج بيانات المستند.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | يحصل على نوع الفهرس الذي يُستخدم له المستخرج. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | يضبط نوع الفهرس الذي يُستخدم له المستخرج. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


يحصل على نوع الفهرس الذي يُستخدم له المستخرج. القيمة الافتراضية هي GroupDocs.Search.Options.IndexType.NormalIndex.


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


يضبط نوع الفهرس الذي يُستخدم له المستخرج. القيمة الافتراضية هي GroupDocs.Search.Options.IndexType.NormalIndex.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | نوع الفهرس الذي يُستخدم له المستخرج. |
|

