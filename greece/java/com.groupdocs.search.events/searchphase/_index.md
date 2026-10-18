---
title: "SearchPhase"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τις φάσεις αναζήτησης."
type: docs
weight: 24
url: /el/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Αναπαριστά τις φάσεις αναζήτησης.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | Η αντικατάσταση ψευδωνύμου. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | Η διόρθωση διάταξης πληκτρολογίου. |
|
|  | [SpellingCorrection](#SpellingCorrection) | Η διόρθωση ορθογραφίας. |
|
|  | [HomophoneSearch](#HomophoneSearch) | Η αναζήτηση ομοηχητικών. |
|
|  | [SynonymSearch](#SynonymSearch) | Η αναζήτηση συνωνύμων. |
|
|  | [WordFormsSearch](#WordFormsSearch) | Η αναζήτηση μορφών λέξεων. |
|
|  | [FuzzySearch](#FuzzySearch) | Η ασαφής αναζήτηση. |
|
|  | [WildcardMatching](#WildcardMatching) | Η αντιστοίχιση μπαλαντέρ. |
|
|  | [RegexMatching](#RegexMatching) | Η αντιστοίχιση κανονικής έκφρασης. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


Η αντικατάσταση ψευδωνύμου.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


Η διόρθωση διάταξης πληκτρολογίου.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


Η διόρθωση ορθογραφίας.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


Η αναζήτηση ομοηχητικών.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


Η αναζήτηση συνωνύμων.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


Η αναζήτηση μορφών λέξεων.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


Η ασαφής αναζήτηση.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


Η αντιστοίχιση μπαλαντέρ.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


Η αντιστοίχιση κανονικής έκφρασης.


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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
