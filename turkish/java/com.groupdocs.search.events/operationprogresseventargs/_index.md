---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İndeksleme işlemi ilerlemesi güncellendiğinde olayın argümanlarını temsil eder."
type: docs
weight: 18
url: /tr/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

İndeksleme işlemi ilerlemesi güncellendiğinde olayın argümanlarını temsil eder.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | İşlenecek belgelerin toplam sayısını alır. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Başarıyla işlenen belgelerin sayısını alır. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Atlanan belgelerin sayısını alır. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | İlerlemenin yüzdesini alır. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Son işlenen belgenin anahtarını alır. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Son işlenen belgenin yolunu alır. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Son işlenen belgenin durumunu alır. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


İşlenecek belgelerin toplam sayısını alır.


**Returns:**
int - İşlenecek belgelerin toplam sayısı.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Başarıyla işlenen belgelerin sayısını alır.


**Returns:**
int - Başarıyla işlenen belgelerin sayısı.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Atlanan belgelerin sayısını alır.


**Returns:**
int - Atlanan belgelerin sayısı.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


İlerlemenin yüzdesini alır.


**Returns:**
double - İlerlemenin yüzdesi.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Son işlenen belgenin anahtarını alır.


**Returns:**
java.lang.String - Son işlenen belgenin anahtarı.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Son işlenen belgenin yolunu alır.


**Returns:**
java.lang.String - Son işlenen belgenin yolu.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Son işlenen belgenin durumunu alır.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

