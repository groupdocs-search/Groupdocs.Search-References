---
title: "SpellingCorrector"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد واجهة مصحح الإملاء للمصطلحات في الاستعلام."
type: docs
weight: 21
url: /ar/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

يحدد واجهة مصحح الإملاء للمصطلحات في الاستعلام.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCount()](#getCount--) | يحصل على عدد الكلمات الموجودة في هذا الـ SpellingCorrector. |
|
|  | [getWords()](#getWords--) | يحصل على مجموعة الكلمات الموجودة حاليًا في هذا الـ SpellingCorrector. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | يضيف مجموعة الكلمات المحددة إلى هذه النسخة من الـ SpellingCorrector. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | يضيف مجموعة الكلمات المحددة إلى هذه النسخة من الـ SpellingCorrector. |
|
|  | [clear()](#clear--) | يزيل جميع الكلمات من كائن SpellingCorrector. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد الكلمات الموجودة في هذا الـ SpellingCorrector.


**Returns:**
int - عدد الكلمات الموجودة في هذا الـ SpellingCorrector.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


يحصل على مجموعة الكلمات الموجودة حاليًا في هذا الـ SpellingCorrector.


**Returns:**
java.lang.String[] - مجموعة الكلمات.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


يضيف مجموعة الكلمات المحددة إلى هذه النسخة من الـ SpellingCorrector.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمات | java.lang.Iterable<java.lang.String> | مجموعة الكلمات لإضافتها إلى القاموس. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


يضيف مجموعة الكلمات المحددة إلى هذه النسخة من الـ SpellingCorrector.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمات | java.lang.String[] | مجموعة الكلمات لإضافتها إلى القاموس. |
|

### clear() {#clear--}
```
public abstract void clear()
```


يزيل جميع الكلمات من كائن SpellingCorrector.


