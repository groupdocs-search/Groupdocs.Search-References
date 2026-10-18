---
title: "OptimizationProgressEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa ketika kemajuan operasi pengindeksan diperbarui."
type: docs
weight: 19
url: /id/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Mewakili argumen untuk peristiwa ketika kemajuan operasi pengindeksan diperbarui.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | Mendapatkan total jumlah segmen untuk diproses. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Mendapatkan jumlah segmen yang diproses. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Mendapatkan persentase kemajuan. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Mendapatkan total jumlah segmen untuk diproses.


**Returns:**
int - Total jumlah segmen untuk diproses.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Mendapatkan jumlah segmen yang diproses.


**Returns:**
int - Jumlah segmen yang diproses.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Mendapatkan persentase kemajuan.


**Returns:**
double - Persentase kemajuan.

