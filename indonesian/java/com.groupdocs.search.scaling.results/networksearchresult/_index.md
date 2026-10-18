---
title: "NetworkSearchResult"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili hasil pencarian yang cocok dengan kueri pencarian."
type: docs
weight: 14
url: /id/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Mewakili hasil pencarian yang cocok dengan kueri pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Mendapatkan jumlah dokumen yang ditemukan. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Mendapatkan total jumlah kemunculan yang ditemukan. |
|
|  | [getTruncated()](#getTruncated--) | Mendapatkan nilai yang menunjukkan bahwa hasil dipotong. |
|
|  | [getWarnings()](#getWarnings--) | Mendapatkan peringatan yang menjelaskan hasil. |
|
|  | [getStartTime()](#getStartTime--) | Mendapatkan waktu mulai pencarian. |
|
|  | [getEndTime()](#getEndTime--) | Mendapatkan waktu akhir pencarian. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Mendapatkan durasi pencarian dalam detik. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Mendapatkan dokumen yang ditemukan berdasarkan indeks. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator yang mengiterasi koleksi dokumen yang ditemukan. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Mendapatkan token pencarian chunk untuk mencari chunk berikutnya. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Mendapatkan indeks node dari mana hasil diterima. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Mendapatkan jumlah dokumen yang ditemukan.


**Returns:**
int - Jumlah dokumen yang ditemukan.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Mendapatkan total jumlah kemunculan yang ditemukan.


**Returns:**
int - Total jumlah kemunculan yang ditemukan.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Mendapatkan nilai yang menunjukkan bahwa hasil dipotong.


**Returns:**
boolean - Nilai yang menunjukkan bahwa hasil dipotong.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Mendapatkan peringatan yang menjelaskan hasil.


**Returns:**
java.lang.String - Peringatan yang menjelaskan hasil.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Mendapatkan waktu mulai pencarian.


**Returns:**
java.util.Date - Waktu mulai pencarian.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Mendapatkan waktu akhir pencarian.


**Returns:**
java.util.Date - Waktu akhir pencarian.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Mendapatkan durasi pencarian dalam detik.


**Returns:**
double - Durasi pencarian dalam detik.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Mendapatkan dokumen yang ditemukan berdasarkan indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indeks | int | Indeks dokumen yang ditemukan. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Mengembalikan iterator yang mengiterasi koleksi dokumen yang ditemukan.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - Iterator yang dapat digunakan untuk mengiterasi koleksi dokumen yang ditemukan.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Mendapatkan token pencarian chunk untuk mencari chunk berikutnya.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Mendapatkan indeks node dari mana hasil diterima.


**Returns:**
int - Indeks node dari mana hasil diterima.

