---
title: "DocumentImage"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل بيانات صورة المستند."
type: docs
weight: 16
url: /ar/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

يمثل بيانات صورة المستند.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | يحصل على الرقم الترتيبي للصورة في المستند. |
|
|  | [getFields()](#getFields--) | يحصل على الحقول المستخرجة. |
|
|  | [getFrames()](#getFrames--) | يحصل على إطارات الصورة. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


يحصل على الرقم الترتيبي للصورة في المستند.


**Returns:**
int - الرقم الترتيبي للصورة في المستند.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


يحصل على الحقول المستخرجة.


**Returns:**
com.groupdocs.search.common.DocumentField[] - الحقول المستخرجة.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


يحصل على إطارات الصورة.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - إطارات الصورة.

