---
title: "MergeOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Birleştirme işlemi için seçenekler sağlar."
type: docs
weight: 28
url: /tr/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Birleştirme işlemi için seçenekler sağlar.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | MergeOptions sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isAsync()](#isAsync--) | İşlemin asenkron olarak gerçekleştirilme bayrağını alır. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | İşlemin asenkron olarak gerçekleştirilme bayrağını ayarlar. |
|
|  | [getCancellation()](#getCancellation--) | İşlem iptal nesnesini alır. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | İşlem iptal nesnesini ayarlar. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


MergeOptions sınıfının yeni bir örneğini başlatır.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


İşlemin asenkron olarak gerçekleştirilmesinin bayrağını alır. Varsayılan değer  false .


**Returns:**
boolean - İşlemin asenkron olarak gerçekleştirilmesinin bayrağı.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


İşlemin asenkron olarak gerçekleştirilmesinin bayrağını ayarlar. Varsayılan değer  false .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | İşlemin asenkron olarak gerçekleştirilmesinin bayrağı. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


İşlem iptal nesnesini alır. Varsayılan değer  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


İşlem iptal nesnesini ayarlar. Varsayılan değer  null .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | İşlem iptal nesnesi. |
|

