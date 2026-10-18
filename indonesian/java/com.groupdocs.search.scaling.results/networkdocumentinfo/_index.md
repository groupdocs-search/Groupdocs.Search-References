---
title: "NetworkDocumentInfo"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili deskriptor untuk dokumen terindeks dalam jaringan pencarian."
type: docs
weight: 10
url: /id/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Mewakili deskriptor untuk dokumen terindeks dalam jaringan pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Mendapatkan deskriptor untuk dokumen yang diindeks. |
|
|  | [getShardIndex()](#getShardIndex--) | Mendapatkan indeks shard. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Mendapatkan deskriptor untuk dokumen yang diindeks.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Mendapatkan indeks shard.


**Returns:**
int - Indeks shard.

