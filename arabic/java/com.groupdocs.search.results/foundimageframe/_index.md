---
title: "FoundImageFrame"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل إطار صورة تم العثور عليه."
type: docs
weight: 16
url: /ar/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

يمثل إطار صورة تم العثور عليه.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | يحصل على معلومات المستند. |
|
|  | [getImageIndex()](#getImageIndex--) | يحصل على الرقم الترتيبي للصورة في المستند. |
|
|  | [getFrameIndex()](#getFrameIndex--) | يحصل على فهرس الإطار في الصورة. |
|
|  | [getHashDifferences()](#getHashDifferences--) | يحصل على عدد البتات غير المتطابقة في تجزئة الصورة. |
|
|  | [toString()](#toString--) | يعيد  System.String  الذي يمثل الـ  FoundImageFrame  الحالي. |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


يحصل على معلومات المستند.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


يحصل على الرقم الترتيبي للصورة في المستند.


**Returns:**
int - الرقم الترتيبي للصورة في المستند.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


يحصل على فهرس الإطار في الصورة.


**Returns:**
int - فهرس الإطار في الصورة.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


يحصل على عدد البتات غير المتطابقة في تجزئة الصورة.


**Returns:**
int - عدد البتات غير المتطابقة في تجزئة الصورة.

### toString() {#toString--}
```
public abstract String toString()
```


يعيد  System.String  الذي يمثل الـ  FoundImageFrame  الحالي.


**Returns:**
java.lang.String -  System.String  الذي يمثل الـ  FoundImageFrame  الحالي.

