---
title: "DeleteResult"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir dizinden indekslenmiş dosya veya klasörleri silme işleminin sonucunu temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Bir dizinden indekslenmiş dosya veya klasörleri silme işleminin sonucunu temsil eder.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Her yolun silinme sonuçlarını döndürür. |
|
|  | [getTotalCount()](#getTotalCount--) | Silinecek yolların toplam sayısını döndürür. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Başarıyla silinen yolların sayısını döndürür. |
|
|  | [getFailedCount()](#getFailedCount--) | Hatalar nedeniyle silinemeyen yolların sayısını döndürür. |
|
|  | [getErrors()](#getErrors--) | Silme hatalarının açıklamalarını döndürür. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Her yolun silinme sonuçlarını döndürür.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - Her yolun silinme sonuçları.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Silinecek yolların toplam sayısını döndürür.


**Returns:**
int - Silinecek yolların toplam sayısı.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Başarıyla silinen yolların sayısını döndürür.


**Returns:**
int - Başarıyla silinen yolların sayısı.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Hatalar nedeniyle silinemeyen yolların sayısını döndürür.


**Returns:**
int - Hatalar nedeniyle silinemeyen yolların sayısı.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Silme hatalarının açıklamalarını döndürür.


**Returns:**
java.lang.String[] - Silme hatalarının açıklamaları.

