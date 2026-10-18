---
title: "SearchPhase"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज चरणों को दर्शाता है।"
type: docs
weight: 24
url: /hi/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

खोज चरणों को दर्शाता है।

## Fields

| Field | विवरण |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | उपनाम प्रतिस्थापन। |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | कीबोर्ड लेआउट सुधार। |
|
|  | [SpellingCorrection](#SpellingCorrection) | वर्तनी सुधार। |
|
|  | [HomophoneSearch](#HomophoneSearch) | होमोफोन खोज। |
|
|  | [SynonymSearch](#SynonymSearch) | समानार्थक शब्द खोज। |
|
|  | [WordFormsSearch](#WordFormsSearch) | शब्द रूप खोज। |
|
|  | [FuzzySearch](#FuzzySearch) | फ़ज़ी खोज। |
|
|  | [WildcardMatching](#WildcardMatching) | वाइल्डकार्ड मिलान। |
|
|  | [RegexMatching](#RegexMatching) | रेजेक्स मिलान। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


उपनाम प्रतिस्थापन।


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


कीबोर्ड लेआउट सुधार।


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


वर्तनी सुधार।


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


होमोफोन खोज।


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


समानार्थक शब्द खोज।


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


शब्द रूप खोज।


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


फ़ज़ी खोज।


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


वाइल्डकार्ड मिलान।


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


रेजेक्स मिलान।


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
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
