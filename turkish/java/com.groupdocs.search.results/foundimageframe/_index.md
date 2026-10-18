---
title: "FoundImageFrame"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bulunan bir görüntü çerçevesini temsil eder."
type: docs
weight: 16
url: /tr/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Bulunan bir görüntü çerçevesini temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Belge bilgilerini alır. |
|
|  | [getImageIndex()](#getImageIndex--) | Belgedeki görüntünün sıra numarasını alır. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Görüntüdeki çerçevenin indeksini alır. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Görüntü karmasındaki eşleşmeyen bit sayısını alır. |
|
|  | [toString()](#toString--) | Mevcut  FoundImageFrame  i temsil eden bir  System.String  döndürür. |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Belge bilgilerini alır.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Belgedeki görüntünün sıra numarasını alır.


**Returns:**
int - Belgedeki görüntünün sıra numarası.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Görüntüdeki çerçevenin indeksini alır.


**Returns:**
int - Görüntüdeki çerçevenin indeksi.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Görüntü karmasındaki eşleşmeyen bit sayısını alır.


**Returns:**
int - Görüntü karmasındaki eşleşmeyen bit sayısı.

### toString() {#toString--}
```
public abstract String toString()
```


Mevcut  FoundImageFrame  i temsil eden bir  System.String  döndürür.


**Returns:**
java.lang.String - Mevcut  FoundImageFrame  i temsil eden bir  System.String .

