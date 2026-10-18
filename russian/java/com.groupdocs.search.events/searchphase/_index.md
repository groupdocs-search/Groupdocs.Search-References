---
title: "SearchPhase"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет фазы поиска."
type: docs
weight: 24
url: /ru/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

Представляет фазы поиска.

## Fields

| Field | Описание |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | Подстановка псевдонима. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | Коррекция раскладки клавиатуры. |
|
|  | [SpellingCorrection](#SpellingCorrection) | Коррекция орфографии. |
|
|  | [HomophoneSearch](#HomophoneSearch) | Поиск омонимов. |
|
|  | [SynonymSearch](#SynonymSearch) | Поиск синонимов. |
|
|  | [WordFormsSearch](#WordFormsSearch) | Поиск форм слов. |
|
|  | [FuzzySearch](#FuzzySearch) | Не��ткий поиск. |
|
|  | [WildcardMatching](#WildcardMatching) | Сопоставление с подстановочными знаками. |
|
|  | [RegexMatching](#RegexMatching) | Сопоставление по регулярному выражению. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


Подстановка псевдонима.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


Коррекция раскладки клавиатуры.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


Коррекция орфографии.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


Поиск омонимов.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


Поиск синонимов.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


Поиск форм слов.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


Не��ткий поиск.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


Сопоставление с подстановочными знаками.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


Сопоставление по регулярному выражению.


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
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
