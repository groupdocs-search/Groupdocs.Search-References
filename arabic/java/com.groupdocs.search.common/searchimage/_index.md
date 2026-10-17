---
title: "SearchImage"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل صورة للبحث."
type: docs
weight: 29
url: /ar/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

يمثل صورة للبحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | ينشئ صورة من ملف للبحث. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | ينشئ صورة من ملف للبحث. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | ينشئ صورة من تدفق للبحث. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | ينشئ صورة من تدفق للبحث. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


ينشئ صورة من ملف للبحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار ملف الصورة. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


ينشئ صورة من ملف للبحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار ملف الصورة. |
|
|  | imageIndex | int | فهرس الصورة في الصور متعددة الصفحات. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


ينشئ صورة من تدفق للبحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | stream | java.io.InputStream | تدفق الصورة. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


ينشئ صورة من تدفق للبحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | stream | java.io.InputStream | تدفق الصورة. |
|
|  | imageIndex | int | فهرس الصورة في الصور متعددة الصفحات. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

