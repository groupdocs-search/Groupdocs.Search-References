---
title: "SearchPhase"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 단계를 나타냅니다."
type: docs
weight: 24
url: /ko/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

검색 단계를 나타냅니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | 별칭 대체. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | 키보드 레이아웃 교정. |
|
|  | [SpellingCorrection](#SpellingCorrection) | 맞춤법 교정. |
|
|  | [HomophoneSearch](#HomophoneSearch) | 동음이의어 검색. |
|
|  | [SynonymSearch](#SynonymSearch) | 동의어 검색. |
|
|  | [WordFormsSearch](#WordFormsSearch) | 단어 형태 검색. |
|
|  | [FuzzySearch](#FuzzySearch) | 퍼지 검색. |
|
|  | [WildcardMatching](#WildcardMatching) | 와일드카드 매칭. |
|
|  | [RegexMatching](#RegexMatching) | 정규식 매칭. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


별칭 대체.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


키보드 레이아웃 교정.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


맞춤법 교정.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


동음이의어 검색.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


동의어 검색.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


단어 형태 검색.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


퍼지 검색.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


와일드카드 매칭.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


정규식 매칭.


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
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
