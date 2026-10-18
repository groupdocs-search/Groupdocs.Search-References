---
title: "DataExtractedEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belge veri çıkarma işlemi tamamlandığında olayın argümanlarını temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.search.scaling.events/dataextractedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DataExtractedEventArgs extends EventArgs
```

Belge veri çıkarma işlemi tamamlandığında olayın argümanlarını temsil eder.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getExtractorIndex()](#getExtractorIndex--) | Çıkarıcı indeksini alır. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Belge anahtarını alır. |
|
### getExtractorIndex() {#getExtractorIndex--}
```
public final int getExtractorIndex()
```


Çıkarıcı indeksini alır.


**Returns:**
int - Çıkarıcı indeksi.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Belge anahtarını alır.


**Returns:**
java.lang.String - Belge anahtarı.

