---
title: "ErrorOccurredEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa ketika terjadi kesalahan pada salah satu node jaringan pencarian."
type: docs
weight: 13
url: /id/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Mewakili argumen untuk peristiwa ketika terjadi kesalahan pada salah satu node jaringan pencarian.

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Mendapatkan indeks node jaringan pencarian. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Mendapatkan indeks layanan node jaringan pencarian. |
|
|  | [getMessage()](#getMessage--) | Mendapatkan pesan kesalahan. |
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

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Mendapatkan pesan kesalahan.


**Returns:**
java.lang.String - Pesan kesalahan.

