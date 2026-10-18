---
title: "IndexErrorEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa ketika terjadi kesalahan indeks."
type: docs
weight: 16
url: /id/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Mewakili argumen untuk peristiwa ketika terjadi kesalahan indeks.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getMessage()](#getMessage--) | Mendapatkan pesan kesalahan. |
|
|  | [isCritical()](#isCritical--) | Mendapatkan flag yang menunjukkan bahwa kesalahan yang terjadi bersifat kritis dan indeks harus dimulai ulang. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Mendapatkan pesan kesalahan.


**Returns:**
java.lang.String - Pesan kesalahan.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Mendapatkan flag yang menunjukkan bahwa kesalahan yang terjadi bersifat kritis dan indeks harus dimulai ulang.


**Returns:**
boolean - Flag yang menunjukkan bahwa kesalahan yang terjadi bersifat kritis dan indeks harus dimulai ulang.

