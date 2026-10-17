---
title: "SearchPhase"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索阶段。"
type: docs
weight: 24
url: /zh/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

表示搜索阶段。

## Fields

| Field | 描述 |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | 别名替换。 |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | 键盘布局校正。 |
|
|  | [SpellingCorrection](#SpellingCorrection) | 拼写校正。 |
|
|  | [HomophoneSearch](#HomophoneSearch) | 同音词搜索。 |
|
|  | [SynonymSearch](#SynonymSearch) | 同义词搜索。 |
|
|  | [WordFormsSearch](#WordFormsSearch) | 词形搜索。 |
|
|  | [FuzzySearch](#FuzzySearch) | 模糊搜索。 |
|
|  | [WildcardMatching](#WildcardMatching) | 通配符匹配。 |
|
|  | [RegexMatching](#RegexMatching) | 正则表达式匹配。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


别名替换。


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


键盘布局校正。


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


拼写校正。


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


同音词搜索。


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


同义词搜索。


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


词形搜索。


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


模糊搜索。


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


通配符匹配。


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


正则表达式匹配。


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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
