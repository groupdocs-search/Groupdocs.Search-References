---
title: "OperationProgressEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa ketika kemajuan operasi pengindeksan diperbarui."
type: docs
weight: 18
url: /id/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Mewakili argumen untuk peristiwa ketika kemajuan operasi pengindeksan diperbarui.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | Mendapatkan total jumlah dokumen untuk diproses. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Mendapatkan jumlah dokumen yang berhasil diproses. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Mendapatkan jumlah dokumen yang dilewati. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Mendapatkan persentase kemajuan. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Mendapatkan kunci dokumen terakhir yang diproses. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Mendapatkan jalur dokumen terakhir yang diproses. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Mendapatkan status dokumen terakhir yang diproses. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Mendapatkan total jumlah dokumen untuk diproses.


**Returns:**
int - Total jumlah dokumen untuk diproses.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Mendapatkan jumlah dokumen yang berhasil diproses.


**Returns:**
int - Jumlah dokumen yang berhasil diproses.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Mendapatkan jumlah dokumen yang dilewati.


**Returns:**
int - Jumlah dokumen yang dilewati.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Mendapatkan persentase kemajuan.


**Returns:**
double - Persentase kemajuan.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Mendapatkan kunci dokumen terakhir yang diproses.


**Returns:**
java.lang.String - Kunci dokumen terakhir yang diproses.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Mendapatkan jalur dokumen terakhir yang diproses.


**Returns:**
java.lang.String - Jalur dokumen terakhir yang diproses.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Mendapatkan status dokumen terakhir yang diproses.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

