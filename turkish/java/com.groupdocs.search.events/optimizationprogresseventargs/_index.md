---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İndeksleme işlemi ilerlemesi güncellendiğinde olayın argümanlarını temsil eder."
type: docs
weight: 19
url: /tr/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

İndeksleme işlemi ilerlemesi güncellendiğinde olayın argümanlarını temsil eder.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | İşleme için toplam segment sayısını alır. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | İşlenen segment sayısını alır. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | İlerlemenin yüzdesini alır. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


İşleme için toplam segment sayısını alır.


**Returns:**
int - İşleme için toplam segment sayısı.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


İşlenen segment sayısını alır.


**Returns:**
int - İşlenen segment sayısı.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


İlerlemenin yüzdesini alır.


**Returns:**
double - İlerlemenin yüzdesi.

