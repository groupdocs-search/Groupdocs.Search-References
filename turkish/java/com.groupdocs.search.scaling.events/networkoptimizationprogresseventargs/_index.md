---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Optimizasyon işleminin ilerleme değişikliği olayının argümanlarını temsil eder."
type: docs
weight: 15
url: /tr/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Optimizasyon işleminin ilerleme değişikliği olayının argümanlarını temsil eder.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Arama ağı düğümünün dizinini alır. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Arama ağı düğüm hizmetinin dizinini alır. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | İşlenen segment sayısını alır. |
|
|  | [getTotalSegments()](#getTotalSegments--) | İşleme için toplam segment sayısını alır. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | İlerlemenin yüzdesini alır. |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


İşlenen segment sayısını alır.


**Returns:**
int - İşlenen segment sayısı.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


İşleme için toplam segment sayısını alır.


**Returns:**
int - İşleme için toplam segment sayısı.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


İlerlemenin yüzdesini alır.


**Returns:**
double - İlerlemenin yüzdesi.

