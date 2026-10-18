---
title: "SearchPhase"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de zoekfasen voor."
type: docs
weight: 24
url: /nl/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Stelt de zoekfasen voor.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | De aliasvervanging. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | De correctie van de toetsenbordindeling. |
|
|  | [SpellingCorrection](#SpellingCorrection) | De spellingcorrectie. |
|
|  | [HomophoneSearch](#HomophoneSearch) | De homofoonzoeking. |
|
|  | [SynonymSearch](#SynonymSearch) | De synoniemenzoeking. |
|
|  | [WordFormsSearch](#WordFormsSearch) | De zoekopdracht naar woordvormen. |
|
|  | [FuzzySearch](#FuzzySearch) | De fuzzy-zoekopdracht. |
|
|  | [WildcardMatching](#WildcardMatching) | De wildcardovereenkomst. |
|
|  | [RegexMatching](#RegexMatching) | De regexovereenkomst. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


De aliasvervanging.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


De correctie van de toetsenbordindeling.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


De spellingcorrectie.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


De homofoonzoeking.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


De synoniemenzoeking.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


De zoekopdracht naar woordvormen.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


De fuzzy-zoekopdracht.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


De wildcardovereenkomst.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


De regexovereenkomst.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
