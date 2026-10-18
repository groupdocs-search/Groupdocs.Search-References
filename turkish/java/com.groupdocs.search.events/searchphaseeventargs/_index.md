---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama aşaması değişim olaylarının argümanlarını temsil eder."
type: docs
weight: 21
url: /tr/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Arama aşaması değişim olaylarının argümanlarını temsil eder.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Arama aşamasını alır. |
|
|  | [getQuery()](#getQuery--) | Mevcut aramanın başlangıç sorgusunu alır. |
|
|  | [getWords()](#getWords--) | Mevcut aşamada elde edilen kelimeleri alır. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Arama aşamasını alır.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Mevcut aramanın başlangıç sorgusunu alır.


**Returns:**
java.lang.String - Mevcut aramanın başlangıç sorgusu.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Mevcut aşamada elde edilen kelimeleri alır.


**Returns:**
java.lang.String[] - Mevcut aşamada elde edilen kelimeler.

