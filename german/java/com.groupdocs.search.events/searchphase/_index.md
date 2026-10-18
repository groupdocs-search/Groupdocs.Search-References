---
title: "SearchPhase"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Suchphasen dar."
type: docs
weight: 24
url: /de/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Stellt die Suchphasen dar.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | Die Alias-Substitution. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | Die Korrektur der Tastaturbelegung. |
|
|  | [SpellingCorrection](#SpellingCorrection) | Die Rechtschreibkorrektur. |
|
|  | [HomophoneSearch](#HomophoneSearch) | Die Homophon-Suche. |
|
|  | [SynonymSearch](#SynonymSearch) | Die Synonymsuche. |
|
|  | [WordFormsSearch](#WordFormsSearch) | Die Suche nach Wortformen. |
|
|  | [FuzzySearch](#FuzzySearch) | Die unscharfe Suche. |
|
|  | [WildcardMatching](#WildcardMatching) | Die Platzhaltersuche. |
|
|  | [RegexMatching](#RegexMatching) | Die Regex-Übereinstimmung. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


Die Alias-Substitution.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


Die Korrektur der Tastaturbelegung.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


Die Rechtschreibkorrektur.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


Die Homophon-Suche.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


Die Synonymsuche.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


Die Suche nach Wortformen.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


Die unscharfe Suche.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


Die Platzhaltersuche.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


Die Regex-Übereinstimmung.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
