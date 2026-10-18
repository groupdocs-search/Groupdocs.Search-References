---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama sorgusuyla eşleşen bir arama sonucunu temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Arama sorgusuyla eşleşen bir arama sonucunu temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Bulunan belge sayısını alır. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Bulunan toplam oluşum sayısını alır. |
|
|  | [getTruncated()](#getTruncated--) | Sonucun kesildiğini gösteren bir değeri alır. |
|
|  | [getWarnings()](#getWarnings--) | Sonucu açıklayan uyarıları alır. |
|
|  | [getStartTime()](#getStartTime--) | Aramanın başlangıç zamanını alır. |
|
|  | [getEndTime()](#getEndTime--) | Aramanın bitiş zamanını alır. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Aramanın süresini saniye cinsinden alır. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | İndeksle bulunan belgeyi alır. |
|
|  | [iterator()](#iterator--) | Bulunan belgelerin koleksiyonunda dolaşan bir yineleyici döndürür. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Sonraki parçayı aramak için bir chunk arama token'ı alır. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Sonucun alındığı düğümün indeksini alır. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Bulunan belge sayısını alır.


**Returns:**
int - Bulunan belge sayısı.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Bulunan toplam oluşum sayısını alır.


**Returns:**
int - Bulunan toplam oluşum sayısı.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Sonucun kesildiğini gösteren bir değeri alır.


**Returns:**
boolean - Sonucun kesildiğini gösteren bir değer.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Sonucu açıklayan uyarıları alır.


**Returns:**
java.lang.String - Sonucu açıklayan uyarılar.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Aramanın başlangıç zamanını alır.


**Returns:**
java.util.Date - Aramanın başlangıç zamanı.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Aramanın bitiş zamanını alır.


**Returns:**
java.util.Date - Aramanın bitiş zamanı.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Aramanın süresini saniye cinsinden alır.


**Returns:**
double - Aramanın süresi saniye cinsinden.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


İndeksle bulunan belgeyi alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indeks | int | Bulunan bir belgenin indeksi. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Bulunan belgelerin koleksiyonunda dolaşan bir yineleyici döndürür.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - Bulunan belgelerin koleksiyonunda dolaşmak için kullanılabilecek bir yineleyici.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Sonraki parçayı aramak için bir chunk arama token'ı alır.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Sonucun alındığı düğümün indeksini alır.


**Returns:**
int - Sonucun alındığı düğümün indeksi.

