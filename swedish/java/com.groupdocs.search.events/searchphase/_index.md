---
title: "SearchPhase"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar sökfaserna."
type: docs
weight: 24
url: /sv/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Representerar sökfaserna.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | Alias‑substitutionen. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | Korrigeringen av tangentbordslayouten. |
|
|  | [SpellingCorrection](#SpellingCorrection) | Stavningskorrigeringen. |
|
|  | [HomophoneSearch](#HomophoneSearch) | Homofonssökningen. |
|
|  | [SynonymSearch](#SynonymSearch) | Synonymsökningen. |
|
|  | [WordFormsSearch](#WordFormsSearch) | Ordformsökningen. |
|
|  | [FuzzySearch](#FuzzySearch) | Fuzzy‑sökningen. |
|
|  | [WildcardMatching](#WildcardMatching) | Wildcard‑matchning. |
|
|  | [RegexMatching](#RegexMatching) | Regex‑matchning. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


Alias‑substitutionen.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


Korrigeringen av tangentbordslayouten.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


Stavningskorrigeringen.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


Homofonssökningen.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


Synonymsökningen.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


Ordformsökningen.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


Fuzzy‑sökningen.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


Wildcard‑matchning.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


Regex‑matchning.


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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
