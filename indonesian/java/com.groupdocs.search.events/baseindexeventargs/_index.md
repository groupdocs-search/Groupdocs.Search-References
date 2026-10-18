---
title: "BaseIndexEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili kelas dasar argumen peristiwa."
type: docs
weight: 10
url: /id/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Mewakili kelas dasar argumen peristiwa.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getTime()](#getTime--) | Mendapatkan waktu suatu peristiwa. |
|
|  | [getIndexId()](#getIndexId--) | Mendapatkan ID indeks. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Mendapatkan folder indeks. |
|
|  | [getStatus()](#getStatus--) | Mendapatkan status indeks. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Mendapatkan waktu suatu peristiwa.


**Returns:**
java.util.Date - Waktu suatu peristiwa.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Mendapatkan ID indeks.


**Returns:**
java.util.UUID - ID indeks.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Mendapatkan folder indeks.


**Returns:**
java.lang.String - Folder indeks.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Mendapatkan status indeks.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

