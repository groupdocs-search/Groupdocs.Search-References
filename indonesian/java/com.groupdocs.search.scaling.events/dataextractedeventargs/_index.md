---
title: "DataExtractedEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa ketika ekstraksi data dokumen selesai."
type: docs
weight: 10
url: /id/java/com.groupdocs.search.scaling.events/dataextractedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DataExtractedEventArgs extends EventArgs
```

Mewakili argumen untuk peristiwa ketika ekstraksi data dokumen selesai.

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getExtractorIndex()](#getExtractorIndex--) | Mendapatkan indeks ekstraktor. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Mendapatkan kunci dokumen. |
|
### getExtractorIndex() {#getExtractorIndex--}
```
public final int getExtractorIndex()
```


Mendapatkan indeks ekstraktor.


**Returns:**
int - Indeks ekstraktor.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Mendapatkan kunci dokumen.


**Returns:**
java.lang.String - Kunci dokumen.

