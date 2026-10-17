---
title: "ImagePreparingEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث بدء إعداد الصورة."
type: docs
weight: 15
url: /ar/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

يمثل المعلمات لحدث بدء إعداد الصورة.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | يحصل على مفتاح المستند. |
|
|  | [getInnerPath()](#getInnerPath--) | يحصل على المسار الداخلي لمستند متداخل. |
|
|  | [getImageIndex()](#getImageIndex--) | يحصل على الرقم الترتيبي للصورة في المستند. |
|
|  | [getImageFrames()](#getImageFrames--) | يحصل على إطارات الصورة. |
|
|  | [getImageStream()](#getImageStream--) | يحصل على تدفق الصورة. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


يحصل على مفتاح المستند.


**Returns:**
java.lang.String - مفتاح المستند.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


يحصل على المسار الداخلي لمستند متداخل.


**Returns:**
java.lang.String[] - المسار الداخلي لمستند متداخل.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


يحصل على الرقم الترتيبي للصورة في المستند.


**Returns:**
int - الرقم الترتيبي للصورة في المستند.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


يحصل على إطارات الصورة.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - إطارات الصورة.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


يحصل على تدفق الصورة.


**Returns:**
java.io.InputStream - تدفق الصورة.

