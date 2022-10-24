---
title: SearchPhase
second_title: GroupDocs.Search for Java API Reference
description: Represents the search phases.
type: docs
weight: 23
url: /java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Represents the search phases.
## Fields

| Field | Description |
| --- | --- |
| [AliasSubstitution](#AliasSubstitution) | The alias substitution. |
| [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | The keyboard layout correction. |
| [SpellingCorrection](#SpellingCorrection) | The spelling correction. |
| [HomophoneSearch](#HomophoneSearch) | The homophone search. |
| [SynonymSearch](#SynonymSearch) | The synonym search. |
| [WordFormsSearch](#WordFormsSearch) | The word forms search. |
| [FuzzySearch](#FuzzySearch) | The fuzzy search. |
| [WildcardMatching](#WildcardMatching) | The wildcard matching. |
| [RegexMatching](#RegexMatching) | The regex matching. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


The alias substitution.

### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


The keyboard layout correction.

### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


The spelling correction.

### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


The homophone search.

### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


The synonym search.

### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


The word forms search.

### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


The fuzzy search.

### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


The wildcard matching.

### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


The regex matching.

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
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
