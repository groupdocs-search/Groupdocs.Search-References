---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama ağının bir düğümünde bir hata oluştuğunda olayın argümanlarını temsil eder."
type: docs
weight: 13
url: /tr/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Arama ağının bir düğümünde bir hata oluştuğunda olayın argümanlarını temsil eder.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Arama ağı düğümünün dizinini alır. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Arama ağı düğüm hizmetinin dizinini alır. |
|
|  | [getMessage()](#getMessage--) | Hata mesajını alır. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Arama ağı düğümünün dizinini alır.


**Returns:**
int - Arama ağı düğümünün dizini.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Arama ağı düğüm hizmetinin dizinini alır.


**Returns:**
int - Arama ağı düğüm hizmetinin dizini.

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Hata mesajını alır.


**Returns:**
java.lang.String - Hata mesajı.

