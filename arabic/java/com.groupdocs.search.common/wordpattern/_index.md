---
title: "WordPattern"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نمط كلمة لاستخدامه في بحث الكلمات ذات الأحرف البديلة."
type: docs
weight: 34
url: /ar/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

يمثل نمط كلمة لاستخدامه في بحث الكلمات ذات الأحرف البديلة.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | يُنشئ مثيلًا جديدًا من الفئة  WordPattern . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | يضيف سلسلة إلى نمط الكلمة. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | يضيف حرفًا إلى نمط الكلمة. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | يضيف حرفًا واحدًا كبديل إلى نمط الكلمة. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | يضيف حرفًا واحدًا أو لا شيء كبديل إلى نمط الكلمة. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | يضيف صفر أو أكثر من الأحرف كبديل إلى نمط الكلمة. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | يضيف حرفًا واحدًا أو أكثر كبديل إلى نمط الكلمة. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | يضيف بديلًا إلى نمط الكلمة. |
|
|  | [toString()](#toString--) | يرجع  System.String  الذي يمثل الـ  WordPattern  الحالي. |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


يُنشئ مثيلًا جديدًا من الفئة  WordPattern .


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


يضيف سلسلة إلى نمط الكلمة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | نص | java.lang.String | السلسلة المراد إضافتها. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


يضيف حرفًا إلى نمط الكلمة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | حرف | char | الحرف المراد إضافته. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


يضيف حرفًا واحدًا كبديل إلى نمط الكلمة.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


يضيف حرفًا واحدًا أو لا شيء كبديل إلى نمط الكلمة.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


يضيف صفر أو أكثر من الأحرف كبديل إلى نمط الكلمة.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


يضيف حرفًا واحدًا أو أكثر كبديل إلى نمط الكلمة.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


يضيف بديلًا إلى نمط الكلمة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | min | int | الحد الأدنى لعدد الأحرف. |
|
|  | max | int | الحد الأقصى لعدد الأحرف. |
|

### toString() {#toString--}
```
public String toString()
```


يرجع  System.String  الذي يمثل الـ  WordPattern  الحالي.


**Returns:**
java.lang.String - سلسلة System.String تمثل نمط WordPattern الحالي.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
