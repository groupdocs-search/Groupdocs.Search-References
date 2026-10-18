---
title: "DocumentDeletedEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa ketika penghapusan dokumen selesai."
type: docs
weight: 11
url: /id/java/com.groupdocs.search.scaling.events/documentdeletedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentDeletedEventArgs extends EventArgs
```

Mewakili argumen untuk peristiwa ketika penghapusan dokumen selesai.

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Mendapatkan indeks shard. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Mendapatkan kunci dokumen. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Mendapatkan indeks shard.


**Returns:**
int - Indeks shard.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Mendapatkan kunci dokumen.


**Returns:**
java.lang.String - Kunci dokumen.

