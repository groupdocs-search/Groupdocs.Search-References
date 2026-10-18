---
title: "PathDeleteResult"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Dizinden bir indekslenmiş dosya veya klasörü silme işleminin sonucunu temsil eder."
type: docs
weight: 18
url: /tr/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Dizinden bir indekslenmiş dosya veya klasörü silme işleminin sonucunu temsil eder.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Silme işleminin başarı göstergesini döndürür. |
|
|  | [getError()](#getError--) | Silme hatasının bir açıklamasını döndürür. |
|
|  | [getPath()](#getPath--) | Silinecek dosya veya klasörün yolunu döndürür. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Silme işleminin başarı göstergesini döndürür.


**Returns:**
boolean -  true  silme işlemi başarılıysa; aksi takdirde  false  döndürür.

### getError() {#getError--}
```
public final String getError()
```


Silme hatasının bir açıklamasını döndürür.


**Returns:**
java.lang.String - Silme hatasının bir açıklaması.

### getPath() {#getPath--}
```
public final String getPath()
```


Silinecek dosya veya klasörün yolunu döndürür.


**Returns:**
java.lang.String - Silinecek dosya veya klasörün yolu.

