---
title: "SearchPhase"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les phases de recherche."
type: docs
weight: 24
url: /fr/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Représente les phases de recherche.

## Fields

| Field | Description |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | La substitution d'alias. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | La correction de la disposition du clavier. |
|
|  | [SpellingCorrection](#SpellingCorrection) | La correction orthographique. |
|
|  | [HomophoneSearch](#HomophoneSearch) | La recherche d'homophones. |
|
|  | [SynonymSearch](#SynonymSearch) | La recherche de synonymes. |
|
|  | [WordFormsSearch](#WordFormsSearch) | La recherche de formes de mots. |
|
|  | [FuzzySearch](#FuzzySearch) | La recherche floue. |
|
|  | [WildcardMatching](#WildcardMatching) | La correspondance avec des caractères génériques. |
|
|  | [RegexMatching](#RegexMatching) | La correspondance d'expressions régulières. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


La substitution d'alias.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


La correction de la disposition du clavier.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


La correction orthographique.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


La recherche d'homophones.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


La recherche de synonymes.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


La recherche de formes de mots.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


La recherche floue.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


La correspondance avec des caractères génériques.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


La correspondance d'expressions régulières.


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
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
