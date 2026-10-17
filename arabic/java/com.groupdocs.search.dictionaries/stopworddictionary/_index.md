---
title: "StopWordDictionary"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحدد واجهة قاموس كلمات التوقف."
type: docs
weight: 22
url: /ar/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

يحدد واجهة قاموس كلمات التوقف.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCount()](#getCount--) | يحصل على عدد الكلمات الوقفية الموجودة في StopWordDictionary . |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | يضيف مجموعة الكلمات المحددة إلى هذه النسخة من الـ StopWordDictionary . |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | يضيف مجموعة الكلمات المحددة إلى هذه النسخة من الـ StopWordDictionary . |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | يزيل مجموعة الكلمات المحددة من هذه النسخة من الـ StopWordDictionary . |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | يزيل مجموعة الكلمات المحددة من هذه النسخة من الـ StopWordDictionary . |
|
|  | [contains(String word)](#contains-java.lang.String-) | يحدد ما إذا كان كائن StopWordDictionary يحتوي على الكلمة المحددة. |
|
|  | [clear()](#clear--) | يزيل جميع الكلمات من كائن StopWordDictionary . |
|
|  | [iterator()](#iterator--) | يعيد مكرراً يتنقل عبر المجموعة. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


يحصل على عدد الكلمات الوقفية الموجودة في StopWordDictionary .


**Returns:**
int - عدد الكلمات الوقفية في القاموس.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


يضيف مجموعة الكلمات المحددة إلى هذه النسخة من الـ StopWordDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمات | java.lang.Iterable<java.lang.String> | مجموعة الكلمات لإضافتها إلى القاموس. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


يضيف مجموعة الكلمات المحددة إلى هذه النسخة من الـ StopWordDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمات | java.lang.String[] | مجموعة الكلمات لإضافتها إلى القاموس. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


يزيل مجموعة الكلمات المحددة من هذه النسخة من الـ StopWordDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمات | java.lang.Iterable<java.lang.String> | مجموعة الكلمات المراد إزالتها. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


يزيل مجموعة الكلمات المحددة من هذه النسخة من الـ StopWordDictionary .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمات | java.lang.String[] | مجموعة الكلمات المراد إزالتها. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


يحدد ما إذا كان كائن StopWordDictionary يحتوي على الكلمة المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | كلمة | java.lang.String | الكلمة للبحث عنها في كائن StopWordDictionary . |
|

**Returns:**
boolean - true إذا كان كائن StopWordDictionary يحتوي على الكلمة المحددة؛ وإلا false .

### clear() {#clear--}
```
public abstract void clear()
```


يزيل جميع الكلمات من كائن StopWordDictionary .


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


يعيد مكرراً يتنقل عبر المجموعة.


**Returns:**
java.util.Iterator<java.lang.String> - مكرّر يمكن استخدامه للتنقل عبر المجموعة.

