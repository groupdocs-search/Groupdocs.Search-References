---
title: "NetworkIndexingProgressEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa perubahan kemajuan operasi pengindeksan."
type: docs
weight: 14
url: /id/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Mewakili argumen untuk peristiwa perubahan kemajuan operasi pengindeksan.

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Mendapatkan indeks node jaringan pencarian. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Mendapatkan indeks layanan node jaringan pencarian. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Mendapatkan jumlah dokumen yang diproses. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | Mendapatkan total jumlah dokumen untuk diproses. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Mendapatkan persentase kemajuan. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Mendapatkan indeks node jaringan pencarian.


**Returns:**
int - Indeks node jaringan pencarian.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Mendapatkan indeks layanan node jaringan pencarian.


**Returns:**
int - Indeks layanan node jaringan pencarian.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Mendapatkan jumlah dokumen yang diproses.


**Returns:**
int - Jumlah dokumen yang diproses.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Mendapatkan total jumlah dokumen untuk diproses.


**Returns:**
int - Total jumlah dokumen untuk diproses.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Mendapatkan persentase kemajuan.


**Returns:**
double - Persentase kemajuan.

