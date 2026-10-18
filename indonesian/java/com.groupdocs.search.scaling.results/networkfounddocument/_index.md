---
title: "NetworkFoundDocument"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili dokumen yang ditemukan dalam jaringan pencarian."
type: docs
weight: 11
url: /id/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Mewakili dokumen yang ditemukan dalam jaringan pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Mendapatkan dokumen yang ditemukan. |
|
|  | [getShardIndex()](#getShardIndex--) | Mendapatkan indeks shard. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Mendapatkan dokumen yang ditemukan.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Mendapatkan indeks shard.


**Returns:**
int - Indeks shard.

