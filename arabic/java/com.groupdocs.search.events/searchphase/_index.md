---
title: "SearchPhase"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مراحل البحث."
type: docs
weight: 24
url: /ar/java/com.groupdocs.search.events/searchphase/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchPhase extends Enum<SearchPhase>
```

يمثل مراحل البحث.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [AliasSubstitution](#AliasSubstitution) | استبدال الاسم المستعار. |
|
|  | [KeyboardLayoutCorrection](#KeyboardLayoutCorrection) | تصحيح تخطيط لوحة المفاتيح. |
|
|  | [SpellingCorrection](#SpellingCorrection) | تصحيح الإملاء. |
|
|  | [HomophoneSearch](#HomophoneSearch) | بحث المتجانسات الصوتية. |
|
|  | [SynonymSearch](#SynonymSearch) | بحث المرادفات. |
|
|  | [WordFormsSearch](#WordFormsSearch) | بحث صيغ الكلمات. |
|
|  | [FuzzySearch](#FuzzySearch) | البحث الضبابي. |
|
|  | [WildcardMatching](#WildcardMatching) | مطابقة الأحرف البديلة. |
|
|  | [RegexMatching](#RegexMatching) | مطابقة التعبير النمطي. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### AliasSubstitution {#AliasSubstitution}
```
public static final SearchPhase AliasSubstitution
```


استبدال الاسم المستعار.


### KeyboardLayoutCorrection {#KeyboardLayoutCorrection}
```
public static final SearchPhase KeyboardLayoutCorrection
```


تصحيح تخطيط لوحة المفاتيح.


### SpellingCorrection {#SpellingCorrection}
```
public static final SearchPhase SpellingCorrection
```


تصحيح الإملاء.


### HomophoneSearch {#HomophoneSearch}
```
public static final SearchPhase HomophoneSearch
```


بحث المتجانسات الصوتية.


### SynonymSearch {#SynonymSearch}
```
public static final SearchPhase SynonymSearch
```


بحث المرادفات.


### WordFormsSearch {#WordFormsSearch}
```
public static final SearchPhase WordFormsSearch
```


بحث صيغ الكلمات.


### FuzzySearch {#FuzzySearch}
```
public static final SearchPhase FuzzySearch
```


البحث الضبابي.


### WildcardMatching {#WildcardMatching}
```
public static final SearchPhase WildcardMatching
```


مطابقة الأحرف البديلة.


### RegexMatching {#RegexMatching}
```
public static final SearchPhase RegexMatching
```


مطابقة التعبير النمطي.


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
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase)
