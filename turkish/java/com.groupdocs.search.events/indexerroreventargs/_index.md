---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İndeks hatası oluştuğunda olayın argümanlarını temsil eder."
type: docs
weight: 16
url: /tr/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

İndeks hatası oluştuğunda olayın argümanlarını temsil eder.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getMessage()](#getMessage--) | Hata mesajını alır. |
|
|  | [isCritical()](#isCritical--) | Hatanın kritik olduğunu ve indeksin yeniden başlatılması gerektiğini gösteren bir bayrağı alır. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Hata mesajını alır.


**Returns:**
java.lang.String - Hata mesajı.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Hatanın kritik olduğunu ve indeksin yeniden başlatılması gerektiğini gösteren bir bayrağı alır.


**Returns:**
boolean - Hatanın kritik olduğunu ve indeksin yeniden başlatılması gerektiğini gösteren bayrak.

