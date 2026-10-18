---
title: "NetworkOptimizationProgressEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa perubahan kemajuan operasi optimasi."
type: docs
weight: 15
url: /id/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Mewakili argumen untuk peristiwa perubahan kemajuan operasi optimasi.

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Mendapatkan indeks node jaringan pencarian. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Mendapatkan indeks layanan node jaringan pencarian. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Mendapatkan jumlah segmen yang diproses. |
|
|  | [getTotalSegments()](#getTotalSegments--) | Mendapatkan total jumlah segmen untuk diproses. |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Mendapatkan jumlah segmen yang diproses.


**Returns:**
int - Jumlah segmen yang diproses.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Mendapatkan total jumlah segmen untuk diproses.


**Returns:**
int - Total jumlah segmen untuk diproses.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Mendapatkan persentase kemajuan.


**Returns:**
double - Persentase kemajuan.

