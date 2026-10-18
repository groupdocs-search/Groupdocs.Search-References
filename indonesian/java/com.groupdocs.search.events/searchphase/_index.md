---
title: "SearchPhase"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili fase-fase pencarian."
type: docs
weight: 24
url: /id/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Mewakili fase-fase pencarian.

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | Penggantian alias. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | Koreksi tata letak keyboard. |
|
|  | [SpellingCorrection](#SpellingCorrection) | Koreksi ejaan. |
|
|  | [HomophoneSearch](#HomophoneSearch) | Pencarian homofon. |
|
|  | [SynonymSearch](#SynonymSearch) | Pencarian sinonim. |
|
|  | [WordFormsSearch](#WordFormsSearch) | Pencarian bentuk kata. |
|
|  | [FuzzySearch](#FuzzySearch) | Pencarian fuzzy. |
|
|  | [WildcardMatching](#WildcardMatching) | Pencocokan wildcard. |
|
|  | [RegexMatching](#RegexMatching) | Pencocokan regex. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


Penggantian alias.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


Koreksi tata letak keyboard.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


Koreksi ejaan.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


Pencarian homofon.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


Pencarian sinonim.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


Pencarian bentuk kata.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


Pencarian fuzzy.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


Pencocokan wildcard.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


Pencocokan regex.


### values() {#values--}
```
public static SearchPhase[] values()
```




**Returns:**
com.groupdocs.search.events.SearchPhase[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static SearchPhase valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
