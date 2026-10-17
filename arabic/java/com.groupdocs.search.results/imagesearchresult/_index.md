---
title: "ImageSearchResult"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نتيجة بحث عكسي عن صورة."
type: docs
weight: 17
url: /ar/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

يمثل نتيجة بحث عكسي عن صورة.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | يحصل على عدد الصور التي تم العثور عليها. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | يحصل على الصورة الموجودة حسب الفهرس. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


يحصل على عدد الصور التي تم العثور عليها.


**Returns:**
int - عدد الصور التي تم العثور عليها.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


يحصل على الصورة الموجودة حسب الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | الفهرس | int | فهرس الصورة التي تم العثور عليها. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

