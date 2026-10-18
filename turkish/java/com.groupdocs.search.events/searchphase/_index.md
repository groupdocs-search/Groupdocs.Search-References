---
title: "SearchPhase"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama aşamalarını temsil eder."
type: docs
weight: 24
url: /tr/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Arama aşamalarını temsil eder.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | Takma ad değişimi. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | Klavye düzeni düzeltmesi. |
|
|  | [SpellingCorrection](#SpellingCorrection) | Yazım düzeltmesi. |
|
|  | [HomophoneSearch](#HomophoneSearch) | Eşsesli arama. |
|
|  | [SynonymSearch](#SynonymSearch) | Eşanlamlı arama. |
|
|  | [WordFormsSearch](#WordFormsSearch) | Kelime biçimleri araması. |
|
|  | [FuzzySearch](#FuzzySearch) | Bulanık arama. |
|
|  | [WildcardMatching](#WildcardMatching) | Joker karakter eşleştirme. |
|
|  | [RegexMatching](#RegexMatching) | Düzenli ifade eşleştirme. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


Takma ad değişimi.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


Klavye düzeni düzeltmesi.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


Yazım düzeltmesi.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


Eşsesli arama.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


Eşanlamlı arama.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


Kelime biçimleri araması.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


Bulanık arama.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


Joker karakter eşleştirme.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


Düzenli ifade eşleştirme.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
