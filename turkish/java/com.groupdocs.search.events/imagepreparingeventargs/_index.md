---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Görsel hazırlama başlangıcı olayının argümanlarını temsil eder."
type: docs
weight: 15
url: /tr/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Görsel hazırlama başlangıcı olayının argümanlarını temsil eder.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Belge anahtarını alır. |
|
|  | [getInnerPath()](#getInnerPath--) | İç içe bir belgenin iç yolunu alır. |
|
|  | [getImageIndex()](#getImageIndex--) | Belgedeki görüntünün sıra numarasını alır. |
|
|  | [getImageFrames()](#getImageFrames--) | Görüntü karelerini alır. |
|
|  | [getImageStream()](#getImageStream--) | Görüntü akışını alır. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Belge anahtarını alır.


**Returns:**
java.lang.String - Belge anahtarı.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


İç içe bir belgenin iç yolunu alır.


**Returns:**
java.lang.String[] - İç içe bir belgenin iç yolu.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Belgedeki görüntünün sıra numarasını alır.


**Returns:**
int - Belgedeki görüntünün sıra numarası.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Görüntü karelerini alır.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Görüntü kareleri.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Görüntü akışını alır.


**Returns:**
java.io.InputStream - Görüntü akışı.

