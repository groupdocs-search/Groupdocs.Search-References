---
title: "TextStorageSettings"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل إعدادات تخزين النص."
type: docs
weight: 42
url: /ar/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

يمثل إعدادات تخزين النص.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | ينشئ مثيلاً جديداً من الفئة TextStorageSettings. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCompression()](#getCompression--) | يحصل على ضغط تخزين النص. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | يضبط ضغط تخزين النص. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


ينشئ مثيلاً جديداً من الفئة TextStorageSettings.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | ضغط تخزين النص. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


يحصل على ضغط تخزين النص. القيمة الافتراضية هي Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


يضبط ضغط تخزين النص. القيمة الافتراضية هي Compression.Normal.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | ضغط تخزين النص. |
|

