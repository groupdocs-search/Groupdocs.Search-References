---
title: "SearchPhase"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta le fasi di ricerca."
type: docs
weight: 24
url: /it/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Rappresenta le fasi di ricerca.

## Fields

| Field | Descrizione |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | La sostituzione dell'alias. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | La correzione del layout della tastiera. |
|
|  | [SpellingCorrection](#SpellingCorrection) | La correzione ortografica. |
|
|  | [HomophoneSearch](#HomophoneSearch) | La ricerca di omofoni. |
|
|  | [SynonymSearch](#SynonymSearch) | La ricerca di sinonimi. |
|
|  | [WordFormsSearch](#WordFormsSearch) | La ricerca delle forme delle parole. |
|
|  | [FuzzySearch](#FuzzySearch) | La ricerca fuzzy. |
|
|  | [WildcardMatching](#WildcardMatching) | La corrispondenza con caratteri jolly. |
|
|  | [RegexMatching](#RegexMatching) | La corrispondenza regex. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


La sostituzione dell'alias.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


La correzione del layout della tastiera.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


La correzione ortografica.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


La ricerca di omofoni.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


La ricerca di sinonimi.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


La ricerca delle forme delle parole.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


La ricerca fuzzy.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


La corrispondenza con caratteri jolly.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


La corrispondenza regex.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
