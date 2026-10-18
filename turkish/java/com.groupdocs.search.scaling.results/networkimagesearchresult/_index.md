---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama görüntüsüyle eşleşen bir görüntü arama sonucunu temsil eder."
type: docs
weight: 12
url: /tr/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

Arama görüntüsüyle eşleşen bir görüntü arama sonucunu temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | Bulunan resim sayısını alır. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | Bulunan resmi indeksine göre alır. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | Sonraki parçayı aramak için bir parça resim arama belirteci alır. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Sonucun alındığı düğümün indeksini alır. |
|
|  | [getShardIndex()](#getShardIndex--) | Sonucun alındığı shard'ın indeksini alır. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Bulunan resim sayısını alır.


**Returns:**
int - Bulunan görüntü sayısı.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Bulunan resmi indeksine göre alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indeks | int | Bulunan bir görüntünün indeksi. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


Sonraki parçayı aramak için bir parça resim arama belirteci alır.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Sonucun alındığı düğümün indeksini alır.


**Returns:**
int - Sonucun alındığı düğümün indeksi.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Sonucun alındığı shard'ın indeksini alır.


**Returns:**
int - Sonucun alındığı shard'ın indeksi.

