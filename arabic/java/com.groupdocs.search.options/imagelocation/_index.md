---
title: "ImageLocation"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد موقع الصورة."
type: docs
weight: 48
url: /ar/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

يحدد موقع الصورة.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Separate](#Separate) | صورة في ملف منفصل. |
|
|  | [Embedded](#Embedded) | صورة مدمجة في مستند آخر. |
|
|  | [ContainerItem](#ContainerItem) | صورة هي عنصر في ملف حاوية. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


صورة في ملف منفصل.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


صورة مدمجة في مستند آخر.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


صورة هي عنصر في ملف حاوية.


### values() {#values--}
```
public static ImageLocation[] values()
```




**Returns:**
com.groupdocs.search.options.ImageLocation[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ImageLocation valueOf(String name)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
