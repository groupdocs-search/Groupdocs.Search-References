---
title: "NetworkImageSearchResult"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili hasil pencarian gambar yang cocok dengan gambar pencarian."
type: docs
weight: 12
url: /id/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Mewakili hasil pencarian gambar yang cocok dengan gambar pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Mendapatkan jumlah gambar yang ditemukan. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Mendapatkan gambar yang ditemukan berdasarkan indeks. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Mendapatkan token pencarian gambar chunk untuk mencari chunk berikutnya. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Mendapatkan indeks node dari mana hasil diterima. |
|
|  | [getShardIndex()](#getShardIndex--) | Mendapatkan indeks shard dari mana hasil diterima. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Mendapatkan jumlah gambar yang ditemukan.


**Returns:**
int - Jumlah gambar yang ditemukan.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Mendapatkan gambar yang ditemukan berdasarkan indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indeks | int | Indeks gambar yang ditemukan. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Mendapatkan token pencarian gambar chunk untuk mencari chunk berikutnya.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Mendapatkan indeks node dari mana hasil diterima.


**Returns:**
int - Indeks node dari mana hasil diterima.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Mendapatkan indeks shard dari mana hasil diterima.


**Returns:**
int - Indeks shard dari mana hasil diterima.

