---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İndeksleme işleminin ilerleme değişikliği olayının argümanlarını temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

İndeksleme işleminin ilerleme değişikliği olayının argümanlarını temsil eder.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Arama ağı düğümünün dizinini alır. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Arama ağı düğüm hizmetinin dizinini alır. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | İşlenen belgelerin sayısını alır. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | İşlenecek belgelerin toplam sayısını alır. |
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

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


İşlenen belgelerin sayısını alır.


**Returns:**
int - İşlenen belgelerin sayısı.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


İşlenecek belgelerin toplam sayısını alır.


**Returns:**
int - İşlenecek belgelerin toplam sayısı.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


İlerlemenin yüzdesini alır.


**Returns:**
double - İlerlemenin yüzdesi.

