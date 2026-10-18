---
title: "SearchPhaseEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa perubahan fase pencarian."
type: docs
weight: 21
url: /id/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Mewakili argumen untuk peristiwa perubahan fase pencarian.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Mendapatkan fase pencarian. |
|
|  | [getQuery()](#getQuery--) | Mendapatkan kueri awal dari pencarian saat ini. |
|
|  | [getWords()](#getWords--) | Mendapatkan kata-kata yang diperoleh pada fase saat ini. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Mendapatkan fase pencarian.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Mendapatkan kueri awal dari pencarian saat ini.


**Returns:**
java.lang.String - Kueri awal dari pencarian saat ini.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Mendapatkan kata-kata yang diperoleh pada fase saat ini.


**Returns:**
java.lang.String[] - Kata-kata yang diperoleh pada fase saat ini.

